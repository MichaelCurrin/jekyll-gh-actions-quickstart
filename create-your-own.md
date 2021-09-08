---
title: Create your own
---

Get a copy of this template project which you can easily run and host on your GitHub account.

1. Click this button.
    - [![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f)](https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate)
1. Go to your repo's _Actions_ tab and wait for the first workflow to pass.
1. Check your `gh-pages` branch which was created and see that it has a some static HTML files and assets in it.
1. Go to your repo's _Settings_.
1. Enable a GitHub Pages site on the **root** path of the `gh-pages` branch.
1. Go to the _Environment_ section on the right of repo to check the status of the build.
1. When it is done, click _View Deployment_ to open your site URL.

Then you can customize the config, theme, plugins, etc. as you need to.

The Just The Docs theme picks up files automatically and adds them to the navbar, so if you are happy with alphabetical menu, then so you don't have to worry about configuring a navbar. You can also set a custom ordering using `nav_order: 1` to put the page first, as such as homepage.
