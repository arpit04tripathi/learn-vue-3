# Setup

Below are the steps to setup and create new repo

- [Setup](#setup)
  - [Initialize this repo](#initialize-this-repo)
    - [nvm](#nvm)
    - [node](#node)
    - [nvmrc](#nvmrc)
    - [npm create vue](#npm-create-vue)

## Initialize this repo

- [markdown basic syntax](https://www.markdownguide.org/basic-syntax){:target="\_blank"}
- Install nvm [node version manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script){:target="\_blank"}

### nvm

```shell
nvm --version               # current installed nvm version
nvm --help                  # help options
node --version > .nvmrc     # create or update .nvmrc
nvm use                     # user version from .nvmrc
```

### node

```shell
nvm ls-remote               # list of remote node versions
nvm ls-remote --lts
nvm install --lts --default # install lts version and make it default
nvm list                    # list installed versions
nvm use node                # uses latest of installed versions of node
nvm use v20.15.1            # use specific installed version
nvm current                 # current used node version
npm --version               # version of npm
nvm install-latest-npm      # latest npm for current node version
```

### nvmrc

```shell
node --version > .nvmrc     # create or update .nvmrc
nvm current > .nvmrc        # create or update .nvmrc
nvm use                     # user version from .nvmrc
```

### npm create vue

creating new vue-js-3 app using [quickstart](https://vuejs.org/guide/quick-start.html){:target="\_blank"}

```sh
npm create vue@latest; OR
npm init vue@latest; OR
npm init vite@latest;
# and then select `vue`.
```
