## WIP response
When you added "WIP" to the title of this pull request, something changed. Do you see that this pull request is now blocked from merging?

Here's what's happening under-the-hood with the WIP App.

1. The app waits for a change to a pull request title line
2. When a pull request title changes, the app searches for the key-word, **"WIP"**
3. If the search finds "WIP", the app sends a request to GitHub's API to block merging in that pull request

This works by relying heavily on webhooks, payloads, and the GitHub API.

## Definitions
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- Once triggered, the GitHub API sends a payload of data to the user that's [related to their event](https://probot.github.io/docs/webhooks/).
- The GitHub API can send information or make changes to the platform, but only when asked. The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.

When you **remove** WIP from the pull request title, I'll automatically merge the unblocked PR and give you a new set of instructions.

<details><summary>Are apps listening to everything I do? Are they stealing my data?</summary></br>
Nope! Each application will ask you for specific permission to fulfill its purpose. In this case, the app might scan for your issue or pull request context, but only to determine if the content is empty.

This has been happening throughout this course! I've been waiting for you to perform certain expected actions as `Learning Lab`. Applications only respond when certain actions trigger webhooks. For example, if you close this pull request, `WIP` won't do anything.
</details>

### :keyboard: Activity: Continued testing

1. Remove [WIP] from the title of this PR.

<hr>
<h3 align="center">Look for my response in a comment on this PR</h3>
