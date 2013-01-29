source 'https://rubygems.org'


ruby '1.9.3'
# -

gem 'rails', '3.2.11'

#Recommended over Unicorn.
gem 'puma', '~> 1.6.3'
# -
#replacing pg with mongoid for sample
gem 'mongoid'
#gem 'pg'
#gem 'activerecord-postgres-hstore'
#gem 'postgres_ext'
# -

#gem 'activemerchant', require: 'active_merchant'
# -
#gem 'kramdown'
# -





#gem 'newrelic_rpm'
# -

# - used for fragment caching
gem 'redis-rails'
# -

# - require Sinatra for Sidekiq monitoring UI
gem 'sinatra', :require => nil
gem 'sidekiq'
# -

# - Not using, just in here by default
#gem 'jbuilder'
# -

gem 'sitemap_generator'
gem 'state_machine'
gem 'carrierwave'
gem 'fog', '~> 1.3.1'
gem 'mini_magick'
gem 'jquery-rails'
gem 'draper'
gem 'devise'
gem 'rails_admin'
gem 'slim-rails'
gem 'exceptional'

# bummed this has to be available everwhere :-(
gem "mail_view", "~> 1.0.3"

# Gems used only for assets and not required
# in production environments by default.
group :assets do
  gem 'sass-rails',   '~> 3.2.3'
  gem 'compass-rails'
  gem 'coffee-rails', '~> 3.2.1'
  gem 'asset_sync'
  gem 'uglifier', '>= 1.0.3'
end

is_buntu = `uname -a` =~ /buntu/

group :development, :production do
  gem 'foreman'
end

group :development, :staging do
  # - used in `rake n00b`
  # (an interactive CLI app that sets up a dev env)
  gem 'highline'
end

group :development, :test, :staging do
  gem 'faker'
  gem 'factory_girl_rails', '~> 2.0'
  gem 'database_cleaner'
  gem 'launchy'
  gem 'pry'
  gem 'rspec-rails'
  gem 'awesome_print'
  gem 'capybara-screenshot'
end

group :development do
  gem 'heroku'

 
  gem 'guard'
  gem 'guard-rspec'
  gem 'guard-livereload'
  # -

  gem 'libnotify',  require: is_buntu && 'libnotify'
  gem 'rb-inotify', require: is_buntu && 'rb-inotify'
  gem 'ruby-graphviz', require: 'graphviz'
  gem 'brakeman'
  gem 'better_errors'
  gem 'binding_of_caller'
  gem 'mailcatcher'
  gem 'bullet'
  gem 'meta_request', '~> 0.2.1'
end

group :test do
  # - faster and doesn't require Qt
  # like capybara-webkig
  gem 'poltergeist'
  # -

  gem 'simplecov', require: false
  gem 'timecop'
  gem 'shoulda-matchers'
  gem 'turnip'
end
