source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

# Ruby version - 2.3.3 OK
#ruby '2.3.3' || '2.6.4'
#ruby '~> 2.3'
#ruby "2.3.3", :engine => "jruby", :engine_version => "9.1.17.0"
#ruby '2.3.3', :group => [:development, :test]
#ruby '2.6.4', :group => [:production]

#group :production do
#  ENV['CUSTOM_RUBY_VERSION'] = '2.6.4'
#end
#ruby ENV['CUSTOM_RUBY_VERSION'] || '2.3.3'

if ENV["JRUBY"] || RUBY_PLATFORM == "java"
# https://devcenter.heroku.com/articles/ruby-support#ruby-versions
  ruby "2.3.3", :engine => "jruby", :engine_version => "9.1.17.0"
else
  ruby '2.3.3'
end


# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.2.3'

# Use sqlite3 as the database for Active Record
gem 'sqlite3', '~> 1.3.6' , group: [:development, :test]

# PostgreSQ
gem 'pg', '~> 0.18.4', group: [:production]

# Use Puma as the app server
gem 'puma', '~> 3.11'
# Use SCSS for stylesheets
gem 'sass-rails', '5.0.7'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# See https://github.com/rails/execjs#readme for more supported runtimes
gem 'duktape'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.2'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
# gem 'redis', '~> 4.0'
# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use ActiveStorage variant
# gem 'mini_magick', '~> 4.8'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

# Reduces boot times through caching; required in config/boot.rb
gem 'bootsnap', '1.4.1', require: false

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  # Access an interactive console on exception pages or by calling 'console' anywhere in the code.
  gem 'web-console', '>= 3.3.0'
end

group :test do
  # Adds support for Capybara system testing and selenium driver
  gem 'capybara', '3.15.0'
  gem 'selenium-webdriver'
  # Easy installation and use of chromedriver to run system tests with Chrome
  gem 'chromedriver-helper', '1.2.0'
end


# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

# simplecov
gem 'simplecov', '~> 0.17.1', require: false, group: :test
