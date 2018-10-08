Awesome! Now that we have a foundational understanding of Apps, let's talk about how all of this fits together and the greater ecosystem.

If you're not interested and want to get your hands dirty, go ahead and jump down to the activity at the bottom of this comment.

### The SDLC

The software development lifecycle, or **SDLC**, is a complex process. Did you know that the people (aka the ambiguous "they") who categorize things decided there were 6-7 components ("they" haven't reached a consensus) for software-building success?

> Planning -> Requirements -> Design + Prototypes -> Software Development -> Testing -> Deployment -> Operations + Maintenance

If you use GitHub for any part of the SDLC already, chances are you can automate that process via GitHub Apps. If you don't already use GitHub for your whole process, a GitHub App might allow you to build the functionality currently missing, and keep all your software work in one place.

### Apps at GitHub (a history lesson)

Apps on GitHub used to be called bots (have you met my good friend Hubot?).

A bot used to do a few things, like:
- Take up an extra seat on your team's billing account, because they count as a unique user
- Require maintenance and special permissions
- Make independent API requests (more on APIs soon)
- Install with a far greater scope than necessary, granting an entry-point for malicious users to consider attacking

None of these things were ideal. So today, you have two choices, **OAuth Apps** and **GitHub Apps**.

| OAuth App                                                                                                                                                                                                                                              | GitHub App                                                                                                                                                      |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Installed on all repositories a user has access to.                                                                                                                                                                                                    | Connects to a personal account or an organization, but is installed on a specific repository for a specific purpose.                                            |
| Can be connected directly to a specific service, which may perform a variety of behaviors (think CI, Deploy, and Security services).                                                                                                                   | Can be connected to GitHub, Slack, other in-house apps you may have, email programs, or other APIs                                                              |
| Needs hosting.                                                                                                                                                                                                                                         | Needs hosting.                                                                                                                                                  |
| Good for complex processes.                                                                                                                                                                                                                            | Good for specific purposes and simple scripting.                                                                                                                |
| Can be used as an identity provider by enabling a "Login with GitHub" for the authenticated user                                                                                                                                                       | Don't use a GitHub App if you just need a "Login with GitHub" service. But a GitHub App can use a user identification flow to log users in and do other things. |
| should always act as the authenticated GitHub user across all of GitHub (for example, when providing user notifications).                                                                                                                              | Don't build a GitHub App if you only want to act as a GitHub user and do everything that user can do.                                                           |
| Don't build an OAuth App to act as an application for your team or company. OAuth Apps authenticate as a single user, so if one person creates an OAuth App for a company to use, and then they leave the company, no one else will have access to it. | A GitHub App should take actions independent of a user (unless the app is using a user-to-server token).                                                        |
|                                                                                                                                                                                                                                                        |                                                                                                                                                                 |

Remember, this course is all about GitHub Apps.

Looking for an extended Resource? Check out https://developer.github.com/apps/differences-between-apps/

### :keyboard: Activity: Assign yourself


Try to assign me, `Lab`, to this issue. Notice that you can't? That's because I'm not a real user, and I won't act like one, either! You can't tell me what to do! :wink: Look at me reinforcing material. Assign yourself instead.

1. Assign yourself to this issue

<hr>
<h3 align="center">Look for my response in a comment on this issue</h3>
