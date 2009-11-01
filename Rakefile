require 'rake/testtask'

desc 'Default: test'
task :default => :test

desc 'Run thread pool tests.'
Rake::TestTask.new(:test) do |t|
  t.libs << 'test'
  t.pattern = 'test/test_*.rb'
  t.verbose = true
end

task :install do 
  system "gem build thread_pool.gemspec; sudo gem uninstall thread_pool; sudo gem install thread_pool"
end