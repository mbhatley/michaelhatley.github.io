source 'https://rubygems.org'

# Ruby 3.4+ removed these from default gems; jekyll/activesupport/liquid/
# octokit still `require` them without declaring them as dependencies.
gem 'csv'
gem 'benchmark'
gem 'bigdecimal'
gem 'drb'
gem 'mutex_m'
gem 'ostruct'
gem 'rss'

# Was pulled in transitively via the (now-removed) github-pages gem, which
# also pinned liquid to exactly 4.0.3 - a version affected by the Ruby 3.2+
# String#tainted? removal. Pinning jekyll directly lets bundler resolve a
# newer liquid (4.0.4+) that doesn't hit that removed method.
gem 'jekyll', '~> 3.9'
gem 'webrick', '~> 1.8'
gem 'kramdown-parser-gfm'

group :jekyll_plugins do
  gem 'jekyll-feed'
  gem 'jekyll-sitemap'
  gem 'jekyll-redirect-from'
  gem 'jekyll-paginate'
  gem 'jekyll-gist'
  gem 'jemoji'
end
