---
title: About
---

## Using a new Jekyll version

Likebmost Jekyll sites, this one uses a homepage (the `index.md` page), a `Gemfile`, and a config file.

But, there are limitations of the GitHub Pages environment - you cannot use Jekyll 4 or non-standard gems (your Gemfile is ignored) and you cannot add Python, Node, Hugo, etc. to your build flow.

To overcome these limitations, this template project uses a GitHub Actions workflow. Allowing you to specify Jekyll 4 and other gems you want. And use other steps like compiling assets with Node.


## GitHub Actions setup

See [main.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/.github/workflows/main.yml) workflow file.

That uses some _generic_ Actions, to avoid relying into an over-specialized complex Action that does too much (like many other there that do Ruby, Jekyll, building, _and_ deploying). 

The generic steps mean it is easy to see exactly what the steps are doing and to modify the flow. Plus, you can reuse the steps for other projects such as deploying a React site to GH Pages. 

On a commit to the main branch, the CI will do the following:

1. Set up the environment.
2. Build the site.
3. Commit the build output to the repo's [gh-pages](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/tree/gh-pages) branch.

Then that output is served as a static site, since GitHub Pages is enabled in _Settings_.

The CI actually will also run on a PR against the main branch too - it will just skip the last part of committing to the `gh-pages` branch. So you can still use the CI to test your tests and build flow works correctly, without accidentally publishing your feature branch as a deployed site.

See [Actions](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/actions/workflows/main.yml) section on the repo for logs of job runs.


## Theme

A theme is set up in the `Gemfile` and `_config.yml` files.

You can use any Jekyll theme you want - as long as it is compatible with Jekyll 4.

The [just-the-docs](https://pmarsceill.github.io/just-the-docs/) Jekyll theme was chosen for this project, as it gives a lot of functionality without you having to write HTML and CSS. So you can focus on writing in Markdown. 

The theme is designed for presenting content as a documentation website, which is ideal if you have code in a repo and want to host a docs site for it without writing a lot of code. Or if you want to make a bunch of docs sites that are light on configuration and boilerplate code, making them simpler for anyone to maintain and to keep the sites in sync.

To keep your docs _separated_ from your app code, your docs site might be 

- in a `docs` subdirectory instead of the root
- a `docs` branch (still building to `gh-pages`)
- or a separate repo.
