# Security

We take security very seriously. That's why we put an extra effort in encrypting all connections.

All connections are made over HTTPS (Secure HTTP) and WSS (Secure WebSocket).

We also sign all the requests with a *signature* composed of a public and private key so you can ensure the request was made from Prudio servers.

Our infrastructure is hosted at [Heroku](http://heroku.com/) & [Amazon Web Services](http://aws.amazon.com/). We also use [KeyCDN](https://www.keycdn.com/?a=5066) as our CDN provider.

## Slack Scopes

In order to function properly we needs to access some of your team private information.

### Here are the scopes we need to access:

* Confirm identity.
* Access and modify information about your public channels.
* Access information about your team.
* Send messages as "YOUR TEAM".
* Access content in your public channels. (1)
* Access your team's profile information. (2)
* Upload and modify files as you. (3)

### These scopes are needed for:

1. Chats sessions history retrieval.
2. Access your team members name, e-mail and avatar.
3. Allow us to upload files in chat sessions (bots have no access to uploads).

## Found an issue?

Submit your finding to hello@prudio.com

**Please include:**

* A summary of the problem you found
* A step-by-step guide to reproduce the issue
* How to identify you for attribution on this page.

We do not offer money rewards yet. Sorry.
