---
title: About
---

## Limitations of Jekyll on plain GitHub Pages

As most Jekyll sites do, this site uses a homepage (the `index.md` page), a `Gemfile` and a config file..

But, there are limitations of the GitHub Pages environment. You cannot use Jekyll 4 or non-standard gems and you cannot add Python, Node, Hugo, etc. to your build flow.

To overcome these limitations, this template project uses a GitHub Actions workflow.

## GitHub Actions set up

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file.

On a commit to the main branch, the CI does the following:

1. Set up the environment.
2. Build the site.
3. Commit the build output to the repo's [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch. 

Then that output is served as a static site, since GitHub Pages is enabled in _Settings_.

The CI actually also runs on a PR against the main branch too - it just last skips the part of commiting to the `gh-pages` branch. So you can still use the CI to test your tests and build flow works correctly, without accidentally publishing your feature branch as a deployed site.

See [Actions](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/actions/workflows/main.yml) section on the repo for logs of job runs.


## Theme

A theme is set up in the `Gemfile` and `_config.yml` files.

You can use any Jekyll theme you want - as long as it is compatible with Jekyll 4.

The [just-the-docs](https://pmarsceill.github.io/just-the-docs/) Jekyll theme was chosen for this project, as it gives a lot of functionality without you having to write HTML and CSS, so you can focus on writing in markdown. The theme focuses on presenting content for a documentation website - so it is ideal if you have code in a repo and want to host a docs site for it without writing a lot of code. 

To keep your docs separate from your app code, your docs site might be in a `docs` subdirectory, a `docs` branch (still building to `gh-pages` or a separate repo.
