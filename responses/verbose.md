## Set-up

BOT: On registration, create an empty repository called introduction-to-github-apps
BOT: Open the first issue using the text from responses/01_intro-gh-apps.md with the title "Introduction to GitHub Apps"


### Issue 1

01_intro-gh-apps.md - ISSUE

TITLE: Introduction to GitHub Apps
TEXT:

Hey! I'm _so_ excited you're here to learn about Apps! Who doesn't like talking about themselves?

We'll quickly get some foundations out of the way, and then apply that knowledge to some real applications.

### Starter questions

> What's an app(lication)?

In this context, apps are software with a bunch of functionality whose purpose is to make your life easier.

The dictionary calls an application "a formal request to an authority for something," which can also be true in software. When you request a service do something, you're appealing to a greater authority and hoping that it works.

When it doesn't, there's always Twitter. But not in my case! Here, we've got something called the Community Forum. You should leave your concerns there and my human minions will help you fix any issues.

> Why would people use it???

As humans, we're constantly generating data. Photos, text, financial transactions, etc. In your everyday life, you use a ton of software applications to help you create, manage, and sort through all of this data. You might use an e-mail client to compile and **style** your thoughts, a social platform to share and view photos and news, or mobile application to respond to immediate alerts like a social invitation out (your message application) or a financial notification.

Depending on your circumstances, it's likely that your life is just a series of interactions between one application, to another, to another, until you go to bed and use an application to help you wake up in the morning (alarm software) and do it all again.

Really bleak, if you think about it. We should probably all exercise more so we can get away from all this... while listening to music through an application and having our workout tracked so we can monitor ourselves and make sure we're healthy.

... there's no escaping this.

> How does this work on GitHub?

GitHub **is** an app. It comes with a ton of built in functionality to help you manage your work and collaborate. We're hiding processes behind the scenes to help you focus on what's important: your code. And we're consistently releasing new features to make sharing easier.

GitHub Apps allow you to change GitHub's surface-level functionality to automate core actions based on specific behaviors. Whether this is to abstract repetitive processes away, ensure a baseline of behavior, increase community involvement and understanding, or something entirely unexplored, you can change GitHub's default processes to add your own value.

<details><summary>I still don't get the difference.</summary>

Here's a metaphor -- picture an iceberg.
![Iceberg](https://media.istockphoto.com/photos/iceberg-picture-id452595535?k=6&m=452595535&s=612x612&w=0&h=uHzj5baAAZH4osCYXBY5JNRrim-aCqG6TxzQPxAiRrc=)

The iceberg is a GitHub repository.

Much of GitHub's magic is happening under the surface. We're hosting and scaling code and communication, creating and connecting tunnels between you and your favorite integrations, and regularly adding features to the surface to improve your workflow.

Imagine examining this surface every day, and performing the same behaviors. Maybe you need to walk across Iceberg Island™️ every morning to make sure the ice hasn't melted. What if you could use a snowmobile to do that in a fraction of the time? Maybe one day your coworker accidentally arrives to your island with a flamethrower. Flamethrowers are illegal on Iceberg Island™️... obviously. What if you could create a security checkpoint to make sure that dangerous objects are never permitted?

Everyone works differently. Not every island will need a snowmobile, or a security checkpoint. Some might need entirely different tools because they are exploring entirely different research projects.

Many people will continue to explore and build their islands without any extra tools to help them. But those people haven't discovered GitHub Apps.

GitHub Apps are top-layer tools that you can use (and build) to make your regular and repetitive processes easier.

We'll look at some real examples very soon in this course.

</details>
^ Click me for an expanded dialogue!

Helpful resource: https://developer.github.com/apps/about-apps/

Prompt: Leave a comment below to let me know what your favorite app (on GitHub, or that you use in your day to day life!) is.

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
