# frozen_string_literal: true
source "https://rubygems.org"

# Kern
gem "jekyll", "~> 4.3"
gem "jekyll-theme-chirpy", "~> 7.3", ">= 7.3.1"

# Plugins (Pagination, Archive, SEO, Feed, Sitemap)
gem "jekyll-paginate"
gem "jekyll-archives"
gem "jekyll-seo-tag"
gem "jekyll-sitemap"
gem "jekyll-feed"

# Lokal-Entwicklung (Ruby 3.x braucht WEBrick)
group :development do
  gem "webrick", "~> 1.8"
end

# CI-Linkcheck (optional)
group :test do
  gem "html-proofer", "~> 5.0"
end

# Optional: nur für Windows (falls du dort jemals lokal entwickelst)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
  gem "wdm", "~> 0.2.0"
end
