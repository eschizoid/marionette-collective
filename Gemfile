source 'https://rubygems.org'

gem 'json'
gem 'stomp'
gem 'systemu'

group :dev do
  gem 'rake'
  gem "rubocop", :platforms => [:ruby] unless RUBY_VERSION =~ /^1.8/
end

group :test do
  gem 'rdoc'
  gem 'rspec', '~> 2.11.0'
  gem 'mocha', '~> 0.10.0'
  gem 'mcollective-test'
end

if File.exists? "#{__FILE__}.local"
  eval(File.read("#{__FILE__}.local"), binding)
end
