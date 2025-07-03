# frozen_string_literal: true

source "https://rubygems.org"

gem "jekyll-remote-theme", "~> 0.4.3"
gem "jekyll-paginate", "~> 1.1"

gem "html-proofer", "~> 5.0", group: :test

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:mingw, :x64_mingw, :mswin]

group :jekyll_plugins do
  gem "jekyll-gist"
  gem "jekyll-seo-tag"
  gem "jekyll-archives"
  gem "jekyll-sitemap"
  gem "jekyll-include-cache"
end
