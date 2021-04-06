---
layout: default
title: Home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink:
mathjax: true.
---

This is a fork of documentation template "Just the Docs" with MathJax support and a few changes.

## Usage

Just copy this repository to your project's `docs` directory and then set the publishing directory as docs from repository setting as explained in [github pages documents](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site). Everything is in place for github pages usage. However, in case this is how `GemFile` should look like:

```ruby
# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"
gem "github-pages", group: :jekyll_plugins
gem "jekyll-seo-tag", "~> 2.7"
```

Finally, clear the `content` directory and add your own documentation. 

## Local Installation with Bundler

First, we need ruby for jekyll so check [here](https://jekyllrb.com/docs/installation/) for installation. We already have the `Gemfile` so no initialization is necessary.

1. Set the installation directory as local
```bash
bundle config set --local path 'vendor/bundle'
```
2. Install dependencies
```bash
bundle install
```
3. Serve the site locally
```bash
bundle exec jekyll s
```
4. Point your web browser to [http://localhost:4000](http://localhost:4000)

## MathJax Support

Add `mathjax: true` to frontmatter of a page:
```markdown
---
layout: default
title: Home
mathjax: true.
---
```

## Configure Just the Docs

Default directory name is changed to `content` from `docs` since repository itself is used as docs.
- [See configuration options]({{ site.baseurl }}{% link content/configuration.md %})



