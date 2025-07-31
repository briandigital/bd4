source "https://rubygems.org"

# Use the theme name found on RubyGems.org
gem "jekyll-theme-hydeout", "~> 5.0" # This is the current stable for Hydeout theme

# Your _config.yml indicates these plugins.
# We need to explicitly list them and allow for updated versions compatible with Jekyll 4.x.
gem "jekyll", "~> 4.4" # Latest stable Jekyll 4.x
gem "jekyll-feed", "~> 0.17" # Current compatible range
gem "jekyll-gist", "~> 1.5"
gem "jekyll-paginate", "~> 1.1" # This might still be a problem. Jekyll 4.x often requires jekyll-paginate-v2.
                               # We'll try with this first, but be aware it might fail.

# Add other common dependencies if not implicitly pulled by theme/Jekyll
# Explicitly request jekyll-sass-converter 3.x to resolve the conflict
gem "jekyll-sass-converter", "~> 3.1" # Changed from ~> 2.1 or 2.2
gem "rouge", "~> 4.0" # For code highlighting
gem "jekyll-watch", "~> 2.0" # For auto-regeneration in development