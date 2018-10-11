Nice job! Something changed on this repo when you added the "WIP" command. Let's try to get more insight into our app before we look at those changes.

## Breaking down the WIP app components

- **Electricity**: Since this is a Probot app, the power to run comes from hosting and deployment that the creators of the app had to set up. We don't need to worry about this unless we build an app ourselves.
- **Standard behaviors**: GitHub has a list of [documented actions](https://developer.github.com/webhooks/#events) that can alert an app.
- **Location**: Apps are designed to look for those actions in whichever repositories they've been installed.
- **Notification service**: If the expected action occurs, a notification delivery is sent to the app as a webhook payload -- a specific set of data transmitted via GitHub's API.

GitHub Apps will then process this data in the background, responding to the repository with their expected default actions.

For the next exercise, let's add our own notification service to get a better idea of what apps are receiving behind the scenes.

### :keyboard: Activity: Adding a webhook payload delivery service

1. Navigate to https://smee.io/ in another tab or window (keep this tab open for the rest of the course). 
1. Click **Start a new channel**  
1. Copy your unique "Webhook Proxy URL"
1. In [your webhooks settings]({{ repoUrl }}/settings/hooks), click **Add webhook**
1. Paste your unique smee URL in the "Payload URL" field
1. Leave the "Secret" field blank
1. For "Which events would you like to trigger this webhook?", select "Send me everything"
1. Click **Add webhook**
1. Return to this PR and paste your smee URL as a comment

<hr>
<h3 align="center">Look for my response in a comment on this pull request</h3>
