task :default do
  sh "rspec spec/"
end

begin
  require 'jeweler'
  project_name = 'ar_merge'
  Jeweler::Tasks.new do |gem|
    gem.name = project_name
    gem.summary = "Merge 2 ActiveRecords, preserving associations and attributes"
    gem.email = "michael@grosser.it"
    gem.homepage = "https://github.com/grosser/#{project_name}"
    gem.authors = ["Michael Grosser"]
    gem.license = "MIT"
  end

  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler, or one of its dependencies, is not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"
end
