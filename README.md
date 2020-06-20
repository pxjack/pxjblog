# My Blog

This blog is setup using **vuepress-theme-reco**. A simple and beautiful VuePress Blog & Doc theme. 

URL:  https://pxjack.netlify.com/



**Reference Links:**

* [vuepress-theme-reco](https://github.com/vuepress-reco/vuepress-theme-reco)
* [Official blog plugin for VuePress](https://github.com/vuepressjs/vuepress-plugin-blog)



## Setup

First, on my Windows 10 64-bit PC, download and install [Node.js](https://nodejs.org/) and [Yarn](https://yarnpkg.com/).

* node-v12.16.1-x64.msi
* yarn-1.22.0.msi



Then follow the [vuepress-theme-reco](https://github.com/vuepress-reco/vuepress-theme-reco) "Quick start | yarn" to setup.

**yarn**

```bash
# init
yarn global add @vuepress-reco/theme-cli
theme-cli init my-blog

# install
cd my-blog
yarn install

# run
yarn dev

# build
yarn build
```



I updated `package.json` to use latest version. The latest version number can be found :

* VuePress: [CHANGELOG.md](https://github.com/vuejs/vuepress/blob/master/CHANGELOG.md)
* vuepress-theme-reco: [package.json](https://github.com/vuepress-reco/vuepress-theme-reco/blob/develop/package.json)

```json
{
  "devDependencies": {
    "vuepress": "1.3.1",
    "vuepress-theme-reco": "1.2.2"
  },
}
```

Then up run yarn install and upgrade:

```shell
yarn install
yarn upgrade
```



## Deploy

The code repository is on GitHub, deploy to Netlify.com

1. In Netlify, create a new GitHub project, using these settings:

   * Build Command: `yarn build`   OR   `vuepress build docs`
   * Publish directory: `public`
   
2. Click deploy button.

   

[![Netlify Status](https://api.netlify.com/api/v1/badges/ddc80cb2-cf0b-4bae-a27c-571bc52b4107/deploy-status)](https://app.netlify.com/sites/serene-goodall-3e356d/deploys)