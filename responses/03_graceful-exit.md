If you're curious about exactly why this worked, and what webhooks were used under the surface, click the detailed breakdown below.

<details><summary>A detailed breakdown</summary>

- As we dig into the documentation, we should see that the `issues` and `pull_request` events are the webhooks that trigger the GitHub API, since those look for ["opened" GitHub actions](https://developer.github.com/webhooks/#events).
- [This code snippet](https://github.com/behaviorbot/request-info/blob/master/index.js#L7) shows that our app is looking for two specific webhooks, `pull_request.opened` and `issues.opened`.  
- Each event, when triggered, will return a specific [payload](https://developer.github.com/v3/activity/events/types/#events-api-payload-13), which basically just hands you a bunch of data that GitHub requested in the background through its API, for your specific event. Each webhook event has it's own payload example that you can reference in the documentation.  
- In our case, we're looking for [title, body, and user](https://github.com/behaviorbot/request-info/blob/master/index.js#L17).
- The rest is mostly coding logic, which is beyond the scope of our course, but you can see an example of what the app does with that information [here](https://github.com/behaviorbot/request-info/blob/master/lib/PullRequestBodyChecker.js). In this case, it looks to check if the content exists, or if it's equal to the existing default templates without any changes.

</summary>


## Well done!

Congratulations @{{ user.username }}, you've completed the **Introduction to GitHub Apps** course!

![congratulations](https://octodex.github.com/images/welcometocat.png)

## During this course you successfully:

- Learned what GitHub Apps are and how they're useful
- Understood their place in the SDLC and the greater ecosystem
- Were introduced to GitHub's APIs and their role with Apps
- Understood the basic functions of webhooks and how you can interact with them
- Installed two GitHub Probot Apps on our repository


### What's next?

Want to learn more about Probot and GitHub Apps? Below are a few resources that will help you along your journey:
- [Probot Apps](https://probot.github.io/apps/)
- [Probot Documentation](https://probot.github.io/docs/)
- [GitHub Marketplace](https://github.com/marketplace)

### Keep Learning

Want to keep learning? Feel free to [check out our other courses]({{ host }}/courses)?

<hr>
<h3 align="center">I won't respond to this issue, go ahead and close it when finished!</h3>
