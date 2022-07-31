---
title: Create your own
description: Copy this template to your own repos and then deploy to GH Pages
---

1. TOC
{:toc}

## Generate from template

Copy this template to your own repos.

[Use this template][]{: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

Configure the site by updating [\_config.yml](https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/_config.yml) file:

- Update `url` to reflect your own username e.g. `https://MyUsername.github.io`.
- Update `baseurl` to be the name of your repo e.g. `/jekyll-gh-actions-quickstart` or `/my-repo`. If not using a subpath, then use `""`.

[Use this template]: https://github.com/MichaelCurrin/jekyll-themed-site-quickstart/generate


## Deploy with GH Actions and GH Pages

Follow the [Deploy][] steps of this repo's docs to set up the GH Pages site.

[Deploy]: https://github.com/MichaelCurrin/jekyll-gh-actions-quickstart/blob/main/docs/deploy.md


## Configure

- Update the config, such as with your own `title` and `description`.
- Set another theme in `_config.yml` and `Gemfile`.
- Add more plugins to `Gemfile`.


## Update Content

### Pages

Delete the template's Markdown pages.

Add your own Markdown pages.

### Appearance

This template is configured to give all pages the layout of `page` by default. That is defined in the theme as [page.html][], which in turn uses [default.html][].

See the [Just the Docs docs][] for instructions on using the theme and extending such as with CSS. Or look-up the docs for whatever theme you choose.

[Just the Docs docs]: https://just-the-docs.github.io/just-the-docs/

### Navbar

The _Just The Docs_ theme will find files automatically and add them to the navbar for you. So if you are happy with alphabetical menu, then so you don't have to worry about configuring a navbar in the config.

You can also set a custom ordering with a field.

The homepage is set first already because `nav_order` is set to `1`.

```yaml
---
title: Home
layout: default
nav_order: 1
---
```

A second page can be set to `2`.

For more details and nesting pages in directories, see [Navigation structure][] in the theme's docs.

[page.html]: https://github.com/just-the-docs/just-the-docs/blob/master/_layouts/page.html
[default.html]: https://github.com/just-the-docs/just-the-docs/blob/master/_layouts/default.html
[Navigation structure]: https://just-the-docs.github.io/just-the-docs/docs/navigation-structure/
