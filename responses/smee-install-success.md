Nice work adding smee!

## WIP on the surface
When you added "WIP" to the title of this pull request, something changed. Do you see that the pull request's status is "pending" with a yellow dot? This is to block merging while the title includes "WIP".

Let's breakdown how WIP works:

1. The app listens specifically for a change to a pull request title
2. When a pull request title changes, the app searches for the key-word, **"WIP"**
3. If the search finds "WIP", the app sends a request to GitHub's API to block merging in that pull request

Let's use this next activity to find out what's happening behind the scenes.

### :keyboard: Activity: Remove WIP from pull request title
When you made this pull request a work in progress, I took it as a cue to add some good content to this repository! Now that we've got some real work, let's remove the WIP label so that we can merge.

1. To the right of the pull request title, click the **Edit** button
1. Remove `WIP` from the title
1. Click **Save**

<hr>
<h3 align="center">Look for my response in a comment on this pull request</h3>
