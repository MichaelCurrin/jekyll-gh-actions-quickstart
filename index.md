---
title: Home
layout: default
nav_order: 1
---

Source code:

[![MichaelCurrin - jekyll-gh-actions-quickstart](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-gh-actions-quickstart&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart)


## About

As most Jekyll sites do, this site uses a homepage (this `index.md` page), a Gemfile and a config, 

But there are limitations of the GitHub Pages environment (such as no Jekyll 4 or non-standard gems).

To overcome these, this template project uses a GitHub Actions workflow.

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file.

On a commit to the main branch, the CI does the following:

1. Setup the environment.
2. Build the site.
3. Commit the build output to the repo's [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch. 

Then that output is served as a static site, since GitHub Pages is enabled in _Settings_.

The CI actually also runs on a PR against the main branch too - it just last skips the part of commiting to the `gh-pages` branch. So you can still use the CI to test your tests and build flow works correctly, without accidentally publishing your feature branch as a deployed site.

See [Actions](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/actions/workflows/main.yml) section on the repo for logs of job runs.

The [just-the-docs](https://pmarsceill.github.io/just-the-docs/) theme was setup - see the Gemfile and config. You can use any Jekyll theme you want - as long as it is compatiable with Jekyll 4.


## Create your own

Get a copy of this template project which you can easily run and host on your GitHub account.

1. Click this button. [![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f)](https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate)
1. Go to your repo's _Actions_ tab and wait for the first workflow to pass.
1. Check your `gh-pages` branch which was created and see that it has a some static HTML files and assets in it.
1. Go to your repo's _Settings_.
1. Enable a GitHub Pages site on the **root** path of the `gh-pages` branch.
1. Go to the _Environment_ section on the right of repo to check the status of the build.
1. When it is done, click View Deploment to open your site.
