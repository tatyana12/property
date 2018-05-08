source 'https://rubygems.org'

# Declare your gem's dependencies in pwb.gemspec.
# Bundler will treat runtime dependencies like base dependencies, and
# development dependencies will be added by default to the :development group.
gemspec

gem 'rails', '~> 5.1.1'
# Declare any dependencies that are still in development here instead of in
# your gemspec. These might include edge Rails or gems from your path or
# Git. Remember to move these dependencies to your gemspec before releasing
# your gem to rubygems.org.

# gem 'globalize', git: 'https://github.com/globalize/globalize'
# gem 'globalize', github: 'globalize/globalize'
# below needed by above - (in gemspec)
# gem 'activemodel-serializers-xml'
# gem 'globalize-accessors'
# gem 'carrierwave', '>= 1.0.0.rc', '< 2.0'

# To use a debugger
# gem 'byebug', group: [:development, :test]
group :development, :test do
  # gem 'jasmine-rails',        github: 'searls/jasmine-rails'
  # gem 'jasmine-jquery-rails', github: 'travisjeffery/jasmine-jquery-rails'
  # if ENV['TRAVIS']
  #   gem "codeclimate-test-reporter", require: false
  # else
  #   gem 'simplecov',                 require: false
  # end
  gem 'simplecov',                 require: false
  unless ENV['CI']
    # uncommenting below will result in travis ci prompting me to Run `bundle install` elsewhere and add the
    # updated Gemfile.lock to version control
    # gem 'launchy'
    # gem 'annotate'
    # gem 'bumpy'
    # gem 'yard'
    # gem 'redcarpet'
    # gem 'spring'
    # gem 'spring-commands-rspec'
  end

  gem 'launchy'
  # launchy allows me to use save_and_open_page
  # in feature specs to see current page being tested
  gem 'rubocop', require: false
  gem 'pry-byebug'
  gem 'capybara'
  gem 'database_cleaner'
  # , '~> 1.3'
  gem 'rails-controller-testing'
  gem 'factory_girl_rails'
  gem 'poltergeist'
  # , '~> 1.10'
  # gem 'rspec-activemodel-mocks', '~> 1.0'
  gem 'rspec-rails'
  gem 'shoulda-matchers'
  gem 'font-awesome-rails'
  gem 'guard'
  gem 'guard-rspec', require: false
  gem 'zeus'
  gem 'json_spec'

  gem 'rails-perftest'
  gem 'ruby-prof', '0.15.9'
end

group :development do
  gem 'guard-rubocop'
  # below 2 for precompiling assets


# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
# gem 'rails', '~> 5.0.0', '>= 5.0.0.1'
gem 'rails', '~> 5.1.1'
# Use postgresql as the database for Active Record
gem 'pg', '~> 0.18'
# Use Puma as the app server
gem 'puma', '~> 3.0'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.2'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby

# Use jquery as the JavaScript library
gem 'jquery-rails'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
# gem 'redis', '~> 3.0'
# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platform: :mri
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'web-console'
  gem 'listen', '~> 3.0.5'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'

  gem 'closure-compiler'
  gem 'yui-compressor'
end



# /Users/me/.rbenv/versions/2.3.3/lib/ruby/gems/2.3.0/gems/localeapp-2.1.1/lib/localeapp/default_value_handler.rb
# below overwrites I18n::Backend::Base above which causes seeder to break in specs
# gem 'localeapp'


# gem 'bourbon'
gem 'property_web_scraper', github: 'RealEstateWebTools/property_web_scraper'



gem 'globalize', git: 'https://github.com/globalize/globalize'

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]


# , branch: 'link-model-support'
# gem 'globalize', git: 'https://github.com/globalize/globalize'
gem 'paloma', git: 'https://github.com/fredngo/paloma'
# fog-core 1.44.0 requires xmlrpc which is not available in ruby < 2.3...
gem 'fog-core', '1.43.0'
gem 'property_web_scraper', git: 'https://github.com/RealEstateWebTools/property_web_scraper'
end
