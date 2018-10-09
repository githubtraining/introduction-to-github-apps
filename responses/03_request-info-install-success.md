Great job! By following the link, you may have already seen images that teach you how this app works.

If you didn't, here's a summary.

When a user opens an empty issue or pull request, the request info app will do exactly that -- request some more info.

Try to think about which webhook events will be activated when we test this out. Check out the [documentation here](https://developer.github.com/webhooks/). Then, consider what steps the app must know to interact with the GitHub API.

A comprehensive breakdown is below, but I highly recommend that you try and get familiar with that documentation first before I give you any answers! 

<details><summary>How does this magic work?</summary>

As we dig into the documentation, we should see that the `issues` and `pull_request` events are the webhooks that trigger the GitHub API, since those look for ["opened" GitHub actions](https://developer.github.com/webhooks/#events).    

### Technical breakdown
We can also cheat by looking at the guts of the request-info application.
- [This code snippet](https://github.com/behaviorbot/request-info/blob/master/index.js#L7) shows that our app is looking for two specific webhooks, `pull_request.opened` and `issues.opened`.  
- Each event, when triggered, will return a specific [payload](https://developer.github.com/v3/activity/events/types/#events-api-payload-13), which basically just hands you a bunch of data that GitHub requested in the background through its API, for your specific event. Each webhook event has it's own payload example that you can reference in the documentation.  
- In our case, we're looking for [title, body, and user](https://github.com/behaviorbot/request-info/blob/master/index.js#L17).
- The rest is mostly coding logic, which is beyond the scope of our course, but you can see an example of what the app does with that information [here](https://github.com/behaviorbot/request-info/blob/master/lib/PullRequestBodyChecker.js). In this case, it looks to check if the content exists, or if it's equal to the existing default templates without any changes.

</details>

<details><summary> Is the bot listening to everything I do? Is it stealing my data? </summary>

Nope! Each application will ask you for specific permission to accomplish its purpose. [In this case](https://user-images.githubusercontent.com/13326548/46640490-38acad00-cb21-11e8-93c0-88f214be51de.png), the app might scan for your issue or pull request context, but only to determine if the content is empty.

This has been happening throughout this whole course! I've been waiting for you to perform a bunch of expected actions as `Learning Lab`, but other applications only act up when their qualifications are fulfilled. For example, if you close this issue, `request-info` won't do anything. In the meantime, I'll go open a pull request with a blank subject, and we'll see our new friend give you a response.  

</details>

### :keyboard: Activity: Close this issue

1. Close this issue

<hr>
<h3 align="center">Look for my response below!</h3>
