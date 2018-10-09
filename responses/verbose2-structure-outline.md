describe GitHub Apps: their structure, use, and place in the development ecosystem
install a Probot app onto your repository
define a webhook
define an API
explain how events are triggered from actions taken on GitHub
describe how an app consumes and acts on information from a webhook
describe how to customize a default application behavior using a config.yml file


LL Open a PR:
- OP: Introduce apps and place in development ecosystem (heavily reduced).
  - Task: Install WIP Bot
  - LL validates installation
- Comment 1: Describe WIP bot and ask user to trigger its event
  - Task: Edit PR title (Add WIP)
  - LL validates title change
- Comment 2: Define a webhook and what an API is
  - Task: Edit the PR title (remove WIP)
  - LL validates title change
  - LL merges PR and points to next PR

LL open a PR with .github/config.yml
  - OP: Install Request_Info, describe how an app consumes and acts on information from a webhook  
  - Task: Edit the config.yml file
  - LL validates file change
  - LL merges in PR

  - Task: User opens a new issue to see the bot response
  - LL opens congratulations

---------------------
****** VERBOSE ******
---------------------

## Set-up

BOT: On registration, create an empty repository called introduction-to-github-apps
BOT: Open the first PR using the text from responses/01_intro-gh-apps.md with the title "Introduction to GitHub Apps"

### PULL REQUEST ONE

01_intro-gh-apps.md - PR
TITLE: Introduction to GitHub apps
TEXT:

Introduce apps and place in development ecosystem (heavily reduced)...


### :keyboard: Activity: Install the WIP Probot App :tada:

1. Install the [WIP app](https://probot.github.io/apps/wip/) to this repository.
  - Don't install on [ALL of your repositories](https://user-images.githubusercontent.com/13326548/46620238-05dec680-cad9-11e8-8fb6-583dd5d9d5b0.png). This one will do just fine.  

<hr>
<h3 align="center">Look for my response below</h3>

---
USER: Installs WIP.
BOT: Bot validates that the app has been installed.
BOT: Responds with 01_wip-actions.md

01_wip-actions.md - COMMENT
TITLE: Interacting with an App
TEXT:

How does WIP do what it does.
WIP is not a person.

### :keyboard: Activity: Testing an app

1. Add [WIP] to the title of this PR.

<hr>
<h3 align="center">Look for my response in a comment on this PR</h3>

---
USER: edits PR title (Add WIP to title)
BOT: Validates PR title change
BOT: Responds with  01_defining-webhooks-apis.md

01_defining-webhooks-apis.md - COMMENT
TITLE: Definitions
TEXT:

Define a webhook
Define an API

### :keyboard: Activity: Continued testing

1. Remove [WIP] from the title of this PR.

<hr>
<h3 align="center">Look for my response in a comment on this PR</h3>

---
USER: Edits PR title
BOT: Validates title change
BOT: Merges PR
BOT: Posts comment, 01_merge-success.md
BOT: Opens new PR, titled 02_request-info-app-prompt.md

01_merge-success.md - COMMENT
TEXT:

Success message on merge. Go look for the next set of instructions in [this PR](LINK)

---
# PULL REQUEST TWO


02_request-info-app-prompt.md - PR OP

TITLE: Installing another app
TEXT:

For the final exercise, we're going to install another app to this repository and teach you about one last file that you'll find valuable to some GitHub Apps.

### :keyboard: Activity: Install another app  

1. Install the [request info app](https://probot.github.io/apps/request-info/).  

<hr>
<h3 align="center">Look for my response in a comment on this issue</h3>

---
USER: Installs Request Info
BOT: Responds with 02_request-info-install-success.md

TEXT:

Describe how an app consumes and acts on information from a webhook  

### :keyboard: Activity: Change the default message of your config.yml file

1. Edit your pull request to change the default yaml file message for request app

<hr>
<h3 align="center">After you update this PR, i'll go ahead and merge this in for you. Look for my response below</h3>
---
USER: Edits config file
BOT: Validates file change, merges PR.
BOT: Responds with 02_change-config-success.md

Great work! Go open a blank issue to see if your .yml changes took effect!

<hr>
<h3 align="center">Look for my response to your blank issue</h3>
---
USER: Opens new issue, leaves it blank
BOT: Responds to Request Info comment with 03_graceful-exit.md

## Well done!

Congratulations @{{ user.username }}, you've completed the **Introduction to GitHub Apps** course!

![congratulations](https://octodex.github.com/images/welcometocat.png)

## During this course you successfully:

- Learned what GitHub Apps are and how they're useful
- Understood their place in the SDLC and the greater ecosystem
- Were introduced to GitHub's APIs and their role with Apps
- Understood the basic functions of webhooks and how you can interact with them
- Installed two GitHub Probot Apps on our repository


### What's next?

Want to learn more about Probot and GitHub Apps? Below are a few resources that will help you along your journey:
- [Probot Apps](https://probot.github.io/apps/)
- [Probot Documentation](https://probot.github.io/docs/)
- [GitHub Marketplace](https://github.com/marketplace)

### Keep Learning

Want to keep learning? Feel free to [check out our other courses]({{ host }}/courses)?

<hr>
<h3 align="center">I won't respond to this issue, go ahead and close it when finished!</h3>
