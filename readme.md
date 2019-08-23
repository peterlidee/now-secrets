### Now secrets ###
Minimal code reproduction on how to access Now secrets from next, deployed with Now.

To reproduce, add a secret called my_secret to now using now cli
```
now secrets add my_secret 123
```
Then deploy to now: `now`

Open url and check your console, it should say: `my_secret is 123`
