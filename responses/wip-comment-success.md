Nice work adding smee!

## WIP response
When you added "WIP" to the title of this pull request, something changed. Do you see that the pull request's status is "pending" with a yellow dot? This is to block merging while the title includes "WIP".

Here's what's happening under-the-hood with the WIP app.

1. The app listens specifically for a change to a pull request title
2. When a pull request title changes, the app searches for the key-word, **"WIP"**
3. If the search finds "WIP", the app sends a request to GitHub's API to block merging in that pull request

Each application will ask you for specific permission to fulfill its purpose.

This has been happening throughout this course. I've been waiting for you to perform certain expected actions as `Learning Lab`. Applications only respond when certain actions trigger webhooks. For example, if you close this pull request, `WIP` won't do anything.


### :keyboard: Activity: Remove WIP from pull request title
I've made some more changes to this pull request, so it's no longer a work in progress.

1. To the right of the pull request title, click the **Edit** button
1. Remove `WIP` from the title
1. Click **Save**

<hr>
<h3 align="center">Look for my response in a comment on this pull request</h3>
