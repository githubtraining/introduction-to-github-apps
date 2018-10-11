## WIP response
When you added "WIP" to the title of this pull request, something changed. Do you see that the pull request's status is "pending" with and yellow dot? This is to block merging while the title includes "WIP".

Here's what's happening under-the-hood with the WIP app.

1. The app listens specifically for a change to a pull request title
2. When a pull request title changes, the app searches for the key-word, **"WIP"**
3. If the search finds "WIP", the app sends a request to GitHub's API to block merging in that pull request

Each application will ask you for specific permission to fulfill its purpose. In this case, the app might scan for your issue or pull request context, but only to determine if the content is empty.

This has been happening throughout this course. I've been waiting for you to perform certain expected actions as `Learning Lab`. Applications only respond when certain actions trigger webhooks. For example, if you close this pull request, `WIP` won't do anything.

## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- Once triggered, the GitHub API sends a payload of data to a predefined location that's related to the event.
- The GitHub API can send information or make changes to the platform, but only when asked. The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.

When you **remove** WIP from the pull request title, I'll automatically merge the unblocked pull request and give you a new set of instructions.

### :keyboard: Activity: Remove WIP from pull request title

1. To the right of the pull request title, click the **Edit** button
1. Remove `WIP` from the title
1. Click **Save**

<hr>
<h3 align="center">Look for my response in a comment on this pull request</h3>
