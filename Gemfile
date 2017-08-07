# frozen_string_literal: true

source "https://rubygems.org"
gem 'github-pages', group: :jekyll_plugins
gem "rake", "~> 12.0"



group :jekyll_optional_dependencies do
  gem "coderay", "~> 1.1.0"
  gem "jekyll-coffeescript"
  gem "jekyll-docs", :path => "../docs" if Dir.exist?("../docs") && ENV["JEKYLL_VERSION"]
  gem "jekyll-feed", "~> 0.9"
  gem "jekyll-gist"
  gem "jekyll-paginate"
  gem "jekyll-redirect-from"
  gem "kramdown", "~> 1.9"
  gem "mime-types", "~> 3.0"
  gem "rdoc", "~> 5.0"
  gem "toml", "~> 0.1.0"

  platform :ruby, :mswin, :mingw, :x64_mingw do
    gem "classifier-reborn", "~> 2.1.0"
    gem "liquid-c", "~> 3.0"
    gem "pygments.rb", "~> 0.6.0"
    gem "rdiscount", "~> 2.0"
    gem "redcarpet", "~> 3.2", ">= 3.2.3"
    gem "yajl-ruby", "~> 1.2"
  end

  # Windows does not include zoneinfo files, so bundle the tzinfo-data gem
  gem "tzinfo-data", :platforms => [:mingw, :mswin, :x64_mingw, :jruby]
end

#

group :site do
  if ENV["PROOF"]
    gem "html-proofer", "~> 3.4"
  end

  gem "jekyll-avatar"
  gem "jekyll-mentions"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jemoji"
end
