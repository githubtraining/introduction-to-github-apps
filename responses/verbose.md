## Set-up

BOT: On registration, create an empty repository called introduction-to-github-apps
BOT: Open the first issue using the text from responses/01_intro-gh-apps.md with the title "Introduction to GitHub Apps"


### Issue 1

01_intro-gh-apps.md - ISSUE

TITLE: Introduction to GitHub Apps
TEXT:
What's an app?
How does this work on GitHub?
Why would people use it???

<include SDLC ecosystem fit>
"Essentially: If you use GitHub for any part of the SDLC, chances are you can automate the process."

Prompt: Leave a comment below with your favorite app (on GitHub, or that you use in your day to day life!)

---

USER: Leave comment.
BOT: Responds with 01_first-class-actor.md

01_first-class-actor.md - COMMENT

TEXT:

Brief history lesson of how apps/bots work and impact seats.
Permissions are handled differently now.
OAUTH vs GitHub App: https://developer.github.com/apps/differences-between-apps/

Prompt: Try to assign `Lab` to this issue. Notice that you can't? Look at us reinforcing material. Assign yourself instead.   

---

USER: Assigns themselves to the issue
BOT: Responds with 01_anatomy-github-app.md

01_anatomy-github-app.md - COMMENT

TEXT:

Metaphor - Home monitoring system: https://github.com/github/developer-relations/pull/12#discussion_r199652259
Diagram/Picture - Needs making.


Prompt: Close issue.

---

USER: closes issue
BOT: Opens the next PR from responses/02_app-install-response.md. Edits README.md?

### Pull Request 1

02_wip-app-prompt.md - PR

TEXT:

Introduce Probot.

Check out all the cool things you can do: https://probot.github.io/apps/

Hey user, install the WIP app (to this repo only, don't apply it to everything you have access to.)
 - Screenshot

Prompt: Install WIP

---

USER: Installs WIP
BOT: Bot validates that app has been installed. Responds with 02_wip-success.md

02_wip-install-success.md - COMMENT

TEXT:

Now that your app has been installed, let's make sure it works.

Prompt: Change title of PR to [WIP]

---

USER: Changes title. Adds WIP.
BOT: Waits for merge to be blocked. Responds with 02_intro-webhooks.md

02_intro-webhooks.md - COMMENT

TEXT:

Introduce what webhooks are. This webhook alters the [lookthisup] event.

Prompt: Change title of PR, remove WIP.

---

USER: Changes title. Removes WIP.
BOT: Listens for PR success. Responds with 02_intro-apis.md

02_intro-apis.md - COMMENT

TEXT:

Webhook events work because of APIs. When you trigger events, you're communicating with GitHub's API.
[Add Diagram]

Prompt: Merge this PR and we'll go see just how complex these apps can get.

---

### Issue 2

USER: Merges PR.
BOT: Opens new issue with responses/03_reminder-app-prompt.md

03_reminder-app-prompt.md - PR

TEXT: Let's install another App! Last time we used a PR, this time it's an issue. So versatile.

Prompt: Install the reminder app.

---

USER: Installs reminder app.
BOT: Validates installation and responds with 03_reminder-install-success.md

03_reminder-install-success.md - COMMENT

TEXT: Hey you did it. This one is a bit different and will impact different webhooks. Let's test it.

Prompt: Leave a reminder command. Example: Remind me to [do something] in a minute (ideally less time, let's experiment).

---

USER: Writes reminder command.
BOT: Responds to issue comment with 03_arbitrary-webhook.md

03_arbitrary-webhook.md - COMMENT

TEXT:

How does this magic work? How does it persist through time?
Is the bot listening to everything I do? Is it stealing my data? No, watch what happens if you do something the bot isn't designed to look for.

Prompt: Do a specific webhook that's wrong.

---

USER: Does something wrong
BOT: Responds to arbitrary webhook with 03_closing-statement.md

03_closing-statement.md - COMMENT

TEXT:

Look at that! Reminder and WIP didn't do anything, even though you took an action. Remember, it's a security camera that's designed to look into a specific place. The only reason Lab knows this even happened is because we were looking for the specific arbitrary webhook that we assigned you. Surprise! I've been an app this whole time.  

Prompt: Close this issue. You've done it.

---
USER: Closes issue.
BOT: Opens final issue with 04_graceful-exit.md

### Issue 3

04_graceful-exit.md - ISSUE

TEXT:

Well done. Set a reminder to come back and do another course soon! Want to learn how to build a bot? Our next course will be published within a month.
