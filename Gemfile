# frozen_string_literal: true

source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3"

# Chirpy theme
gem "jekyll-theme-chirpy", "~> 7.0", ">= 7.0.1"

# Required plugins for GitHub Pages
group :jekyll_plugins do
  gem "jekyll-paginate", "~> 1.1"
  gem "jekyll-redirect-from", "~> 0.16"
  gem "jekyll-feed", "~> 0.16"
  gem "jekyll-sitemap", "~> 1.4"
  gem "jekyll-spaceship", "~> 0.10.2"
end

# Lock these to prevent breaking changes
gem "tzinfo", ">= 1", "< 3"
gem "tzinfo-data"

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]