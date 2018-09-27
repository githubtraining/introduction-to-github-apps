## Outline (3 separate courses)

### Introduction to GitHub Apps
- Intro to APIs (video?)
  - Ref: https://www.youtube.com/watch?v=s7wmiS2mSXY (one of my favorite instructional videos on YouTube)
  - REST vs. GraphQL
- Intro to Webhooks (video?)
- Intro to GitHub Apps (video?)
  - How do apps fit into the SDLC ecosystem?
  - What is a "first class actor"?
  - Anatomy of a GitHub App (What are the necessary components?)
    - Metaphor: https://github.com/github/developer-relations/pull/12#discussion_r199652259
- Intro to Probot (activity)
  - Existing examples
    - https://probot.github.io/apps/
  - What is it? 
    - How is a Probot app different from a standard GitHub App? 
    - Permissions
  - Installing reminder bot

---

### Building a GitHub App using Probot (basic)

Activity: Triaging GitHub issues (auto-translator) 

- Forming basic API calls and responses
  - REST and GraphQL (course preferences?) 
- Selecting the right Webhook events
  - Reading GitHub docs
  - Unauthenticated Events
- Generating a new app
  - Configuration
  - Testing: Smee, Glitch, and Localtunnel (course preferences) (Choosing what's right for you)
  - Deployment: Glitch, Heroku, Now (course preferences)

---

### Advanced GitHub Apps

Basically, creating an activity or exercise to match each tab from https://probot.github.io/docs/ 

This can be a series of bite-sized challenges that extends the work and activity from our previous auto-labler above?

- HTTP Routes
- Simulating Webhooks
- Logging
- Pagination
- Extensions
- Environment Configuration
- Persistence
- Best Practices
