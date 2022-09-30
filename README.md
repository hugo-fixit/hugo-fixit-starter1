# Hugo FixIt Blog Template (Git)

This is a quick start template for Hugo theme [FixIt](https://github.com/hugo-fixit/FixIt). It uses Git submodule feature to load the theme.

It comes with a basic theme structure and configuration. GitHub action has been set up to deploy the theme to a public GitHub page automatically. Also, there's a cron job to update the theme automatically everyday.

1. Click *Use this template*, and create your repository on GitHub.
2. Once the repository is created, just clone and enjoy it!

## Directory structure

```bash
▸ .github/       # GitHub configuration
▸ .shell/        # shell commands for hugo project, entrance: hugo_main.sh
▸ archetypes/    # page archetypes (like scaffolds of archetypes)
▸ assets/        # css, js, third-party libraries etc.
▸ content/       # markdown files for hugo project
▸ data/          # blog data (allow: yaml, json, toml), e.g. friends.yml
▸ public/        # build directory
▸ static/        # static files, e.g. favicon.ico
▸ themes/        # theme submodules
  config.toml    # configuration of hugo project
```

## Installation

1. Go to [Hugo Releases](https://github.com/gohugoio/hugo/releases) and download the lastest `hugo_extended` version, e.g.

    - `hugo_extended_0.88.1_Windows-64bit.zip`
    - `hugo_extended_0.88.1_macOS-ARM64.tar.gz`

2. Clone your blog source

    ```bash
    # Clone with your own repository url
    git clone --recursive git@github.com:hugo-fixit/hugo-fixit-blog.git
    ```

## Quick Start

There are three ways to start this blog.

### Hugo

```bash
# Development environment
hugo server --disableFastRender --navigateToChanged
# Production environment
hugo server --disableFastRender --navigateToChanged --environment production
```

### Shell

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
