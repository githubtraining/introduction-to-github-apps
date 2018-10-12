## WIP below the surface

Since installation, smee.io has been running patiently in the background and keeping a ledger of each webhook event that we've performed on the repository.

When you edited the pull request title, that triggered a specific type of event.

When that event was triggered, it sent a payload of data to our app. Each type of event delivers a different payload template to the app. When customizing or creating apps, having this knowledge becomes crucial.

## Step 5: Name the event

Can you tell which type of event was sent back to the application when you changed the pull request header?

### :keyboard: Activity: Connecting actions on GitHub to events and payloads

1. Return to your unique smee.io link, accessible via your [settings]({{ repoUrl }}/settings/hooks) if you closed it
1. Identify the webhook event that was triggered. Remember, you edited the pull request title
1. Post the event exactly as it's written in smee.io in a comment on this pull request

<hr>
<h3 align="center">Look for my response in a comment on this pull request</h3>
