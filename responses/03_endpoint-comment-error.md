Nice try! The label creation endpoint, found [here](https://docs.github.com/en/rest/reference/issues#create-a-label), looks like this: `POST /repos/{owner}/{repo}/labels`.

## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- When an event is triggered, the vastly more detailed GitHub API gives the bot an excessive amount of information (as a payload). The bot takes this payload, alters it slightly, and hands it back to GitHub's API, which delivers the change back to your repository.
- The GitHub API can send information that makes changes to the platform, but only when prompted via webhook.
- The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.

## Step 10: See your changes in action 

Now that you've made the change to your `config.yml` file, try to trigger that event to see the changes as a user.

### :keyboard: Activity: Test out your original changes to the config.yml
1. Go open a [blank issue]({{ repoUrl }}/issues/new) to see if the changes you made in your `config.yml` took effect!
