> How does this magic work?

As we dig into the documentation, we should see that the `issue.comment` is the webhook that triggers the GitHub API.

However, for this application, the behavior is slightly different. Generally webhooks call on the API to perform an immediate action.

In this case, returning to leave a comment at a later time adds some complexity beyond what is typically expected. This requires storage as well as GitHub API use.

MORE DETAIL NEEDED WITH WIFI

Each app is

> Is the bot listening to everything I do? Is it stealing my data?

Nope! Each application will ask you for specific permission to accomplish its purpose. In this case, the app might scan for your issue context, but only to seek out the `/reminder` keyword.

You can even test this out! Watch what happens if you do something the bot isn't designed to look for by closing the issue instead.

### :keyboard: Activity: Close this issue

1. Close this issue

<hr>
<h3 align="center">Look for my response in a comment on this issue</h3>
