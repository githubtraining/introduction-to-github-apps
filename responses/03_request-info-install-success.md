## How does it all work?

Great job! By following the link, you may have already seen images that teach you how this app works.

Try to think about which webhook events will activate when we test this out. Was it the opening of an issue, or a comment? When a user opens an empty issue or pull request, the request info app will do exactly that -- request some more info.

### Is the bot listening to everything I do? Is it stealing my data?

Nope! Each application will ask you for specific permission to fulfill its purpose. In this case, the app might scan for your issue or pull request context, but only to determine if the content is empty.

This has been happening throughout this whole course! I've been waiting for you to perform certain expected actions as `Learning Lab`. Applications only respond when certain actions trigger webhooks. For example, if you close this issue, `request-info` won't do anything.

In the meantime, I'll go open a pull request with a blank subject, and we'll see our new friend give you a response.


### :keyboard: Activity: Close this issue

1. Close this issue

<hr>
<h3 align="center">Look for my response below!</h3>
