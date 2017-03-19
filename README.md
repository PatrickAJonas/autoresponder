# Autoresponder

[![Greenkeeper badge](https://badges.greenkeeper.io/probot/autoresponder.svg)](https://greenkeeper.io/)

This is a GitHub Integration built with [probot](https://github.com/probot/probot) that automatically replies to opened GitHub issues with the contents of `.github/ISSUE_REPLY_TEMPLATE.md`.

![](https://cloud.githubusercontent.com/assets/173/23834371/788d330e-0723-11e7-9e71-81d77c01267d.png)

## Deploying to Heroku

0. [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy) - Click this button and pick an **App Name** that Heroku is happy with. Before you can complete this, you'll need config variables from the next step.

0. In another tab, [create an integration](https://github.com/settings/integrations/new) on GitHub, using `https://[yourappname].herokuapp.com/` (replacing `[yourappname]` with the name from step 1) as the **Homepage URL**, **Callback URL**, and **Webhook URL**. The permissions and events that your bot needs access to will depend on what you use it for. Read more about [creating an integration](https://developer.github.com/early-access/integrations/creating-an-integration/).

0. After creating your GitHub integration, go back to the Heroku tab and fill in the configuration variables with the values for the GitHub Integration

0. Create a `.github/ISSUE_REPLY_TEMPLATE.md` file in your repository.
