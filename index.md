---
title: Homepage
layout: default
---

[![MichaelCurrin - jekyll-gh-actions-quickstart](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-gh-actions-quickstart&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart)


## About

This site used a homepage (`index.md`), Gemfile and config, as with most Jekyll sites.

To avoid the limitations of the GitHub Pages environment such as no Jekyll 4 or non-standard gems, this template project uses GitHub Actions to build the site. 

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file.

On a commit, the CI runs to setup the environment, build the site and then commit to the [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch. Then that output is served as static output with GitHub Pages.



## Create your own

1. Click this button. [![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f)](https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate)
1. Wait for the first workflow to complete. Go your _Actions_ tab.
1. Check your `gh-pages` branch which was created and see that it has a some static HTML files and assets in it.
1. Go to your repo _Settings_.
1. Enable a GitHub Pages site on the root of the `gh-pages` branch.
1. Go to the _Environment_ section on the right of repo to check the status of the build.
1. When it is done, click View Deploment to open your site.


## Resources

Pages on my Dev Resources project.

- [Jekyll](https://michaelcurrin.github.io/dev-resources/resources/jekyll/)
- [GitHub Actions](https://michaelcurrin.github.io/dev-resources/resources/ci-cd/github-actions/)
- [GitHub Pages](https://michaelcurrin.github.io/dev-resources/resources/web/github-pages.html)


## Setup locally

This project is not indended to be run locally with a dev server.

If you want to run it locally, I recommend following instructions and setup on this project.

[![MichaelCurrin - jekyll-blog-demo](https://img.shields.io/static/v1?label=MichaelCurrin&message=jekyll-blog-demo&color=blue&logo=github)](https://github.com/MichaelCurrin/jekyll-blog-demo)

It covers installing Ruby, Bundle and project gems locally (including Jekyll). It has a `Gemfile` which you can use to get started.

That uses a plain GH Pages and Jekyll 3.9 approach without GH Actions though.