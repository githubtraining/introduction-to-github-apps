## API endpoints

Nice job!

In the last pull request, we learned that WIP responds to `pull_request` events, before making changes to the merge status.

Request info is watching **two** events, `issues` and `pull_requests`. Remember, though, that these are broad categories. Tons of behaviors can happen to `issues` and `pull_requests`.

Endpoints, accessible only via the API, allow an app to respond to very specific types of behavior, even though it gets notifications for every possibility.  

For request info, the [documentation](https://developer.github.com/v3/activity/events/types/#pullrequestevent) tells us that the `pull_request` event is triggered when a pull request is assigned, unassigned, labeled, unlabeled, opened, edited, closed, reopened, or synchronized.

Since request info responds to blank issues or pull requests, it makes sense that we'd want to narrow our comment responses to the `pull_request.opened` endpoint.

![image](https://user-images.githubusercontent.com/13326548/46848367-3c993300-cd9e-11e8-8542-6138d5e453d9.png)

How does the app respond to a `pull_request.opened` event?

## APIs and Webhooks
APIs and Webhooks go hand in hand, but the distinction between them is important.

- Webhooks are specific "noise" interpreters. They listen for specific events to occur as their trigger.
- When an event is triggered, the vastly more detailed GitHub API gives the bot an excessive amount of information (as a payload). The bot takes this payload, alters it slightly, and hands it back to GitHub's API, which delivers the change back to your repository.
- The GitHub API can send information that makes changes to the platform, but only when prompted via webhook.
- The GitHub API _and_ GitHub's webhooks are both key components of GitHub Apps.


### :keyboard: Activity: Respond with something 


<hr>
<h3 align="center">After you comment, look for my response below</h3>




Great work! Go open a [blank issue]({{ repoUrl }}/issues/new) to see if the changes you made in your `config.yml` took effect!


the config file that you just edited has several optional categories that give us a look into different actions that can be taken from. You changed the comment response, which means that the app can use the
