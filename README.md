# Netlify Identity Demo in Vuejs

## Introduction

The repo [whizjs/netlify-identity-demo-vue](https://github.com/whizjs/netlify-identity-demo-vue) has a demo of how to use Netlify Identity with Vue using the [Netlify Identity widget](https://github.com/netlify/netlify-identity-widget)
that is deployed at <https://netlify-identity-demo-vue.netlify.app/>. 

The demo currently (2023) fails when signup with a CORS error:

```
Access to fetch at 'https://netlify-identity-demo-vue.netlify.com/.netlify/identity/settings' from origin 'https://netlify-identity-demo-vue.netlify.app' has been blocked by CORS policy: Response to preflight request doesn't pass access control check: Redirect is not allowed for a preflight request.
netlify-identity-demo-vue.netlify.com/.netlify/identity/settings:1          Failed to load resource: net::ERR_FAILED
```

This is a fork of the repo.

## Features:
 - Vue.js 3.x in 2019
 - vuex
 - vue-router
 - Netlify Identiy Widget
 - Netlify (hosting) 

## Installation

```
node --version
v16.0.0

npm --version
8.3.2
```

When trying to install the dependencies using node v18.8 and npm 9.2 I with yarn  got the following error:

```bash
[1/2] ⡀ fsevents
warning Error running install script for optional dependency: "/Users/casianorodriguezleon/campus-virtual/2223/learning/netlify-learning/netlify-identity-demo-vue/node_modules/fsevents: Command failed. 
```
When tried with npm it worked with v18! but both the `npm run serve` and `yarn serve` failed. 

When tried npm with node v16 failed but then a `yarn install` succeeded and then `yarn serve` worked.

For production

```
yarn build
```

Lints and fixes files

```
yarn lint
```

## CORS

See [How to enable CORS on a Netlify deployment?](https://stackoverflow.com/questions/62507022/how-to-enable-cors-on-a-netlify-deployment)



## References

* <https://www.netlify.com/blog/2017/09/07/introducing-built-in-identity-service-to-streamline-user-management/>
