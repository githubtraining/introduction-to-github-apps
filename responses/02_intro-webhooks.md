Remember, every time you perform an action on a website you're generating data. For GitHub, many of those standard actions are recognizable as **specific events**, like creating a new issue, or leaving a comment.

Each GitHub App specializes in different **events**, to perform routine behaviors. Remember that it's similar to a security monitoring system, looking for actions like movement or noise in a specific part of your home, and then perfoming a pre-defined action that is triggered from the event.

Here's what's happening under-the-hood with the WIP App.

1. The App waits for a change to a PR subject line.
2. If a PR title changes, the app searches for the key-word, **"WIP"**.
3. If "WIP" is added to a subject, the app will then send a pre-defined request to GitHub's API, to perform a specific behavior.
4. In this case, the GitHub API is used to change the PR behavior and block a merge.

Now let's see what happens when you **remove** WIP from the PR title. Revert your change, and we'll learn more in the next comment.

### :keyboard: Activity: Continued testing

1. Remove [WIP] from the PR title.   

<hr>
<h3 align="center">Look for my response in a comment on this PR</h3>
