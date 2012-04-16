require 'bundler'
require 'rake/testtask'

Bundler::GemHelper.install_tasks

desc 'Run tests.'
Rake::TestTask.new(:test) do |t|
  t.libs << 'lib' << 'test'
  t.pattern = 'test/**/*_test.rb'
  t.verbose = true
end

task :default => [:test]
