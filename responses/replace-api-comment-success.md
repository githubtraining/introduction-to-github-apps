Great work! That's the correct API endpoint. 

## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- When an event is triggered, the vastly more detailed GitHub API gives the bot an excessive amount of information (as a payload). The bot takes this payload, alters it slightly, and hands it back to GitHub's API, which delivers the change back to your repository.
- The GitHub API can send information that makes changes to the platform, but only when prompted via webhook.
- The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.

Go open a [blank issue]({{ repoUrl }}/issues/new) to see if the changes you made in your `config.yml` took effect!
