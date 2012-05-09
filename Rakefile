# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "rack_page_cache"
  gem.homepage = "http://github.com/radiospiel/rack_page_cache"
  gem.license = "MIT"
  gem.summary = %Q{A rack middleware to cache requests in static files, a la Rails' page_cache}
  gem.description = %Q{A rack middleware to cache requests in static files, a la Rails' page_cache}
  gem.email = "eno@open-lab.org"
  gem.authors = ["radiospiel"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/*_test.rb'
  test.verbose = true
end

task :default => :test
