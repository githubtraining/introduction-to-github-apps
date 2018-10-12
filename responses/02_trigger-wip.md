## Triggering GitHub Apps

Actions that a person or tool takes on GitHub can be used to trigger events. Creating an issue, making a commit, or leaving a comment, to name a few, are logged on GitHub. If GitHub doesn't use it, it can still be useful to other applications.

When you install an app, you give the app permission to receive some of this data from GitHub. That data allows the apps to react in ways that are useful to you. You can also allow the app to send information back, or change information completely.

It's important to mention that GitHub Apps are not people. You can't interact with them by doing things like using an @mention, or assigning them to review your work. On the other hand, they can do things that humans can't - like crunch big data, piece together networks of information and find bugs or errors that people wouldn't.

## App components

An app is like a home security system. It's equipped to watch your house at all times, but only notifies you for specific criteria.	When you install a home security system, you need to worry about a few components:

- **Electricity** to have the power to run continuously. You don't want failure when you aren't watching.
- **Standard behaviors** to detect things like movement, noise, and doors opening. You don't want to have to program it to understand these actions -- you want to select how it responds to them.
- A **location** that will be watched.
- A **notification delivery service** -- either to your phone, a dedicated security service, or both.

Just like a home security system, a GitHub App only watches for specific actions, and then responds in predetermined ways.

## Step 2: Trigger the WIP app

**WIP** is a common abbreviation to mean **work in progress**.

The app you've just installed is concerned with one action: changing the title of a pull request. Let's test it out and see what the result is by updating the title of this pull request.

### :keyboard: Activity: Test the app by editing the pull request title

1. To the right of the pull request title, click the **Edit** button
1. Add `WIP` to the beginning of the title
1. Click **Save**

<hr>
<h3 align="center">After changing the title, look for my response in this pull request</h3>
