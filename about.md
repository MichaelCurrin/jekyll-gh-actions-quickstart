---
title: About
---

As most Jekyll sites do, this site uses a homepage (the `index.md` page), a `Gemfile` and a config file.. 

But, there are limitations of the GitHub Pages environment. You cannot use Jekyll 4 or non-standard gems and you cannot add Python, Node, Hugo, etc. to your build flow.

To overcome these, this template project uses a GitHub Actions workflow.

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file.

On a commit to the main branch, the CI does the following:

1. Set up the environment.
2. Build the site.
3. Commit the build output to the repo's [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch. 

Then that output is served as a static site, since GitHub Pages is enabled in _Settings_.

The CI actually also runs on a PR against the main branch too - it just last skips the part of commiting to the `gh-pages` branch. So you can still use the CI to test your tests and build flow works correctly, without accidentally publishing your feature branch as a deployed site.

See [Actions](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/actions/workflows/main.yml) section on the repo for logs of job runs.

The [just-the-docs](https://pmarsceill.github.io/just-the-docs/) theme was set up - see the Gemfile and config. You can use any Jekyll theme you want - as long as it is compatiable with Jekyll 4.
