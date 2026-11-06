# frozen_string_literal: true

source "https://rubygems.org"

gem "jekyll", "~> 4.3"

# Stdlib gems that Ruby 3.4+ no longer loads automatically under Bundler.
gem "erb"
gem "csv"
gem "base64"
gem "bigdecimal"
gem "logger"

group :jekyll_plugins do
  gem "jekyll-paginate"
  gem "jekyll-archives"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-feed"
end

gem "html-proofer", "~> 5.0", group: :test

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]

platforms :windows, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:windows]
