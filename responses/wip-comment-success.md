Perfect! As you might guess, pull_request is a broad event.

In the next exercise, we'll take a look at how apps can take general event payloads and turn those into specific responses via the API.

After you removed WIP from the pull request title, the pull request was unblocked. Now, you're able to merge.

### :keyboard: Activity: Merge
1. Merge this pull request, and delete your branch

> _Sometimes I respond too fast for the page to update! If you perform an expected action and don't see a response from me, wait a few seconds and refresh the page for your next steps._







## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- Once triggered, the GitHub API sends a payload of data to a predefined location that's related to the event.
- The GitHub API can send information or make changes to the platform, but only when asked. The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.
