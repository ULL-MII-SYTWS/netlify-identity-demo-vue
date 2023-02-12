# Netlify Identity Demo in Vuejs

## Introduction

The repo [whizjs/netlify-identity-demo-vue](https://github.com/whizjs/netlify-identity-demo-vue) has a demo of how to use Netlify Identity with Vue using the [Netlify Identity widget](https://github.com/netlify/netlify-identity-widget)
that is deployed at <https://netlify-identity-demo-vue.netlify.app/>. 

The demo currently (2023) fails when signup.

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


## References

* <https://www.netlify.com/blog/2017/09/07/introducing-built-in-identity-service-to-streamline-user-management/>
