<<<<<<< HEAD
#!/usr/bin/env rake
begin
  require 'bundler/setup'
rescue LoadError
  puts 'You must `gem install bundler` and `bundle install` to run rake tasks'
end

# below as per
# https://www.viget.com/articles/rails-engine-testing-with-rspec-capybara-and-factorygirl
APP_RAKEFILE = File.expand_path('../spec/dummy/Rakefile', __FILE__)
load 'rails/tasks/engine.rake'

Bundler::GemHelper.install_tasks

Dir[File.join(File.dirname(__FILE__), 'tasks/**/*.rake')].each { |f| load f }

require 'rspec/core'
require 'rspec/core/rake_task'

desc 'Run all specs in spec directory (excluding plugin specs)'
RSpec::Core::RakeTask.new(spec: 'app:db:test:prepare')

task default: :spec

# require 'rdoc/task'

# RDoc::Task.new(:rdoc) do |rdoc|
#   rdoc.rdoc_dir = 'rdoc'
#   rdoc.title    = 'Pwb'
#   rdoc.options << '--line-numbers'
#   rdoc.rdoc_files.include('README.md')
#   rdoc.rdoc_files.include('lib/**/*.rb')
# end

load 'rails/tasks/statistics.rake'

require 'bundler/gem_tasks'
=======
# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require_relative 'config/application'

Rails.application.load_tasks
>>>>>>> 554139d2104cf80f3d909b8af578654e1d79c3aa
