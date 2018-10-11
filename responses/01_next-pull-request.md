## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- Once triggered, the GitHub API sends a payload of data to a predefined location that's related to the event.
- The GitHub API can send information or make changes to the platform, but only when asked. The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.

Now that we've explored the WIP app, let's move onto what request info can do.

### :keyboard: Activity: Open a pull request
1. Open a pull request [using this link]({{ repoUrl }}/compare/request-info?expand=1), without changing the title or body


<h3 align="center">I'll respond in your new pull request</a></h3>
