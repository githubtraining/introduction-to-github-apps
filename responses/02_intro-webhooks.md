## Triggering GitHub Apps

When you added "WIP" to the title of this pull request, something changed. Do you see that this pull request is now blocked from merging?

When you do things on GitHub, GitHub notices, even if there's no specific reaction. Actions like creating a issue, making a commit, or leaving a comment all create data on GitHub. Even if GitHub doesn't use it, it can be useful to other applications.

When you install an app, you give the app permission to receive some of this data from GitHub. That data allows the apps to react in ways that are useful to you. You can also allow the app to send information back, or change information completely.

Here's what's happening under-the-hood with the WIP App.

1. The app waits for a change to a pull request title line
2. When a pull request title changes, the app searches for the key-word, **"WIP"**
3. If the search finds "WIP", the app sends a request to GitHub's API to block merging in that pull request

### Removing  WIP

Now, let's see what happens when you **remove** WIP from the pull request title.

### :keyboard: Activity: Continued testing

1. Edit the title of the pull request to remove [WIP]

<hr>
<h3 align="center">Look for my response in a comment on this PR</h3>
