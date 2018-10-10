## Triggering GitHub Apps

Actions that a person or tool takes on GitHub can be used to trigger events. Creating a issue, making a commit, or leaving a comment, to name a few, are logged on GitHub. If GitHub doesn't use it, it can still be useful to other applications.

When you install an app, you give the app permission to receive some of this data from GitHub. That data allows the apps to react in ways that are useful to you. You can also allow the app to send information back, or change information completely.

One thing to keep in mind is that GitHub Apps are not people. You can't interact with them by doing things like using an @mention, or assigning them to review your work. GitHub Apps aren't OAuth apps either, which have a different installation flow and often require machine users to act on their behalf. If you'd like to learn more, check out the documentation on [the differences between GitHub and OAuth Apps](https://developer.github.com/apps/differences-between-apps/).

## The WIP app

The app you've just installed is concerned with one action: changing the title of a pull request. Let's test it out and see what the result is by updating the title of this pull request.  

### :keyboard: Activity: Testing an app

1. Add [WIP] to the title of this PR.

<hr>
<h3 align="center">After changing the title, look for my response in a comment on this PR</h3>
