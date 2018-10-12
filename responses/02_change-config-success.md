## API endpoints

Nice job!

In the last pull request, we've learned about webhooks and how the WIP and Request info apps only respond to specific events. Webhooks allow you to build or set up GitHub Apps which subscribe to certain events on GitHub.com When one of those events is triggered, an HTTP POST payload response is sent to the webhook's configured URL. We saw this with our smee webhook.

But webhooks are only one side to this story. To see the other side, meet API endpoints. :wave:

## APIs

API stands for Application Programming Interface. APIs are used to share data or functionality. This is done by making an HTTP request to an API using an **endpoint**, and then receiving a reponse back.

For example, this is the endpoint to create a new pull request; `POST /repos/:owner/:repo/pulls`

When an event is triggered, the vastly more detailed GitHub API gives the bot an excessive amount of information (as a payload). The bot takes this payload, alters it slightly, and hands it back to GitHub's API, which delivers the change back to your repository.


### :keyboard: Activity: Respond with something 


<hr>
<h3 align="center">After you comment, look for my response below</h3>




Great work! Go open a [blank issue]({{ repoUrl }}/issues/new) to see if the changes you made in your `config.yml` took effect!


the config file that you just edited has several optional categories that give us a look into different actions that can be taken from. You changed the comment response, which means that the app can use the
