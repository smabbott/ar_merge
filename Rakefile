desc "Run all specs in spec directory"
task :default do
  options = "--colour --format progress --loadby --reverse"
  files = FileList['spec/**/*_spec.rb']
  system("spec #{options} #{files}")
end

begin
  require 'jeweler'
  project_name = 'ar_merge'
  Jeweler::Tasks.new do |gem|
    gem.name = project_name
    gem.summary = "Merge of 2 ActiveRecords, secure and simple"
    gem.email = "grosser.michael@gmail.com"
    gem.homepage = "http://github.com/grosser/#{project_name}"
    gem.authors = ["Michael Grosser"]
    gem.rubyforge_project = project_name
    gem.add_dependency ['activerecord']
  end

  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler, or one of its dependencies, is not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"
end