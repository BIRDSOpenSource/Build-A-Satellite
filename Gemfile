source 'https://rubygems.org'

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

gem "jekyll", "~> 4.3.4" # installed by `gem jekyll`
gem "just-the-docs", "0.5.4" # pinned to the current release
# gem "just-the-docs"        # always download the latest release

group :jekyll_plugins do
    gem "jekyll-polyglot"
    gem "webrick" # required when using Ruby >= 3 and Jekyll <= 4.2.2
    gem "base64", "~> 0.2.0"