# Readme

This is a fork of documentation template "Just the Docs" with MathJax support and a few changes.

![jtd](https://user-images.githubusercontent.com/896475/47384541-89053c80-d6d5-11e8-98dc-dba16e192de9.gif)

## Installation

Just copy this repository to your project's `docs` directory and then set the publishing directory as docs from repository setting as explained in [github pages documents](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site). Everything is in place for github pages usage. However, in case this is how `GemFile` should look like:

```ruby
# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"
gem "github-pages", group: :jekyll_plugins
gem "jekyll-seo-tag", "~> 2.7"
```

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
