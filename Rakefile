require 'rake/testtask'
require 'rake/rdoctask'

Rake::RDocTask.new do |rd|
  rd.rdoc_files.include("lib/**/*.rb")
#  rd.options << "--ri"
end
  
task :test => :install do 
  require 'rake/runtest'
  Rake.run_tests 'test/ts_dnsruby.rb'
end

task :default => :install do
end

task :install do
  sh "ruby setup.rb"
end

