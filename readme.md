### Now secrets ###
Minimal code reproduction on how to access Now secrets from inside a Next.js app, deployed with Now. Note that this handles the deployment part, not local development.

To solve this I used info from: https://github.com/zeit/next.js/#exposing-configuration-to-the-server--client-side and https://zeit.co/docs/v2/build-step#using-environment-variables-and-secrets Note that I used 2 files: now.json and next.config.js.

To reproduce, add a secret called my_secret to Now using Now cli
```
now secrets add my_secret 123
```
Then deploy to Now: `now`

Open url and check your console, it should say: `my_secret is 123` 
