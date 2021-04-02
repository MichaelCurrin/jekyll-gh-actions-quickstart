---
title: Homepage
layout: default
---

[![MichaelCurrin - jekyll-gh-actions-quickstart](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-gh-actions-quickstart&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart)


## About

This site used a homepage (`index.md`), Gemfile and config, as most Jekyll sites do.

But, to avoid the limitations of the GitHub Pages environment such as no Jekyll 4 or non-standard gems, this template project uses GitHub Actions to build the site. 

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file and see [Actions](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/actions/workflows/main.yml) section for logs of job runs.

On a commit, the CI runs - to setup the environment, build the site and then commit to the [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch. Then that output is served as static output, with GitHub Pages enabled.

The [just-the-docs](https://pmarsceill.github.io/just-the-docs/) theme is setup - see Gemfile and config. You can use any Jekyll theme you want, as long as it is compatiable with Jekyll 4.


## Create your own

Get a copy of this template project which you can easily run and host on your GitHub account.

1. Click this button. [![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f)](https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate)
1. Go to your repo's _Actions_ tab and wait for the first workflow to pass.
1. Check your `gh-pages` branch which was created and see that it has a some static HTML files and assets in it.
1. Go to your repo's _Settings_.
1. Enable a GitHub Pages site on the **root** path of the `gh-pages` branch.
1. Go to the _Environment_ section on the right of repo to check the status of the build.
1. When it is done, click View Deploment to open your site.
