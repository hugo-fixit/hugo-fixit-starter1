---
title: "Hello World"
subtitle: ""
date: 2022-09-29T17:06:11+08:00
tags:
- hello
- FixIt
categories:
- hello
code:
  maxShownLines: 11
# See details front matter: https://fixit.lruihao.cn/theme-documentation-content/#front-matter
---

Welcome to Hugo FixIt! This is your very first post. Head to this [documentation page](https://fixit.lruihao.cn/theme-documentation-basics/) for a complete guidence to get started with the FixIt theme.

<!--more-->

All feedback is welcome! Head over to the [issues](https://github.com/hugo-fixit/FixIt/issues) or [discussions](https://github.com/hugo-fixit/FixIt/discussions) tracker.

## Quick Start

There are three ways to start this blog.

### Hugo

```bash
# Development environment
hugo server --disableFastRender --navigateToChanged
# Production environment
hugo server --disableFastRender --navigateToChanged --environment production
```

## Shell

Run `hugo_main.sh` to choice frequently-used Hugo commands:

```bash
cd .shell && sh hugo_main.sh
```

```text
--------------Hugo Admin--------------
Please enter the serial number to work
--------------------------------------
1. post
2. server
3. server:production
4. build
5. submodule-sync
6. push
--------------------------------------
Press Ctrl+C to stop
```

### NPM

```bash
npm install
# build the blog
npm run build
# run a local debugging server with watch
npm run server
# run a local debugging server in production environment
npm run server:production
# update theme submodules
npm run update:theme
```
