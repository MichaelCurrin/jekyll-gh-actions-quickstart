---
title: Create your own
---

Get a copy of this template project which you can easily run and host on your GitHub account.

## Deploy from template

1. Copy this template to your own repos.
    - [![Use this template](https://img.shields.io/badge/Generate-Use_this_template-2ea44f)](https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate)
1. Configure the site by updating [\_config.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/_config.yml) file. e.g.in particular, set `url` to have your own username and `baseurl` to be 
    - Replace title and description if you want to.
    - Update `url` to reflect your own username e.g. `https://MyUsername.github.io`.
    - Update `baseurl` to be the name of your repo e.g. `/jekyll-gh-actions-quickstart` or `/my-repo`. If not using a subpath, then use `""`.
1. Go to your repo's _Actions_ tab and wait for the first workflow to pass.
1. Check your `gh-pages` branch which was created and see that it has a some static HTML files and assets in it.
1. Go to your repo's _Settings_.
1. Enable a _GitHub Pages_ site on the **root** path of the `gh-pages` branch.
1. Go to the _Environment_ section on the right of repo to check the status of the build.
1. When it is done, click _View Deployment_ to open your site URL.


## Customize

Then you can customize your site as needed.

- Update the config further.
- Set a new theme in `_config.yml` and `Gemfile`.
- Add more plugins to `Gemfile`.


## Content

Add and update Markdown and HTML pages.

### Layout

The template is set up to give all pages the layout of `page` by default, which is define in the theme as [page.html][], which in turn uses [default.html][].

### Navbar

The _Just The Docs_ theme will find files automatically and add them to the navbar for you. So if you are happy with alphabetical menu, then so you don't have to worry about configuring a navbar in the config.

You can also set a custom ordering.

The homepage is set first already because `nav_order` is set to `1`.

```yaml
---
title: Home
layout: default
nav_order: 1
---
```

A second page can be set to `2`.

[page.html]: https://github.com/pmarsceill/just-the-docs/blob/master/_layouts/page.html
[default.html]: https://github.com/pmarsceill/just-the-docs/blob/master/_layouts/default.html
