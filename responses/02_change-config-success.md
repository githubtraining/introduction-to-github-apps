Nice job!

In the last pull request, we learned about webhooks and how the WIP and Request info apps only respond to specific events. Webhooks allow you to build or set up GitHub Apps which subscribe to certain events on GitHub.  When one of those events is triggered, an HTTP POST payload response is sent to the webhook's configured URL. We saw this with our smee webhook.

But webhooks are only one side to this story. To see the other side, meet API endpoints. :wave:

## API endpoints

API stands for Application Programming Interface. APIs are used to share data or functionality. This is done by making an HTTP request to an API using an **endpoint**, and then receiving a reponse back.

For example, this is the endpoint to create a new pull request; `POST /repos/:owner/:repo/pulls`

When an event is triggered, the vastly more detailed GitHub API gives the bot an excessive amount of information (as a payload). The bot takes this payload, alters it slightly, and hands it back to GitHub's API, which delivers the change back to your repository.

## Step 9: Learn more about the GitHub API

### :keyboard: Activity: Discovering endpoints

1. Navigate to [this list](https://developer.github.com/v3/apps/available-endpoints/)
2. Find the endpoint that an app would use to create a label
3. Post that endpoint as a comment

<hr>
<h3 align="center">After you comment, look for my response below</h3>
