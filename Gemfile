source "https://rubygems.org"

# Use the latest github-pages version (232 is the current stable for GitHub builds)
gem "github-pages", "~> 232", group: :jekyll_plugins
gem "minima"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-last-modified-at"
end

# Modernized Windows support to stop the [DEPRECATED] warnings
# This handles tzinfo and wdm correctly for Windows users
platforms :windows do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
  gem "wdm", "~> 0.1.1"
end

# Keep JRuby specific gem separate
platforms :jruby do
  gem "http_parser.rb", "~> 0.6.0"
end

# Essential for Ruby 3.0+ to prevent "cannot load such file -- webrick"
gem "webrick", "~> 1.8"

