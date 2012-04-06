source 'http://rubygems.org'

gem 'rails', '3.2.3'

# Bundle edge Rails instead:
# gem 'rails', :git => 'git://github.com/rails/rails.git'

# Use unicorn as the web server
# gem 'unicorn'


group :development, :test do
  gem "rspec-rails"
  gem "launchy"
  gem "fabrication"
  unless ENV['TRAVIS']
    platforms :ruby do
      gem 'capistrano'
      gem 'linecache19', '0.5.13'
      gem 'ruby-debug-base19', '0.11.26'
      gem 'ruby-debug19', :require => 'ruby-debug'
    end
  end
end


group :test do
  gem "cucumber-rails", require: false
  gem "capybara-webkit"
  gem "database_cleaner"
  gem "guard-rspec"
  gem "guard-cucumber"
  gem "guard-spork"
  gem 'spork'
  gem "growl"
  gem "rb-fsevent"
  gem "simplecov"
  gem "webrat"
  if ENV['TRAVIS']
    gem 'sqlite3-ruby', :require => 'sqlite3'
    gem 'pg'
  end
end

platforms :jruby do
  gem "jruby-openssl"
  gem "activerecord-jdbcmysql-adapter"
  gem "activerecord-jdbcsqlite3-adapter"
  gem "activerecord-jdbcpostgresql-adapter"
end

platforms :ruby do
  gem "mysql2"
#  gem 'sqlite3-ruby', :require => 'sqlite3'
  gem 'pg'
end

group :assets do
  gem 'sass-rails'
  gem 'coffee-rails'
  gem 'uglifier'
end

gem "i18n"
gem 'haml-rails'
gem 'jquery-rails'
gem 'settingslogic'
gem 'coffee-filter'
gem "therubyracer"
gem "bourbon"
