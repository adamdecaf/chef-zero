source "https://rubygems.org"
gemspec

# gem 'rest-client', :git => 'https://github.com/chef/rest-client.git'

group :pedant do
  gem "oc-chef-pedant", :git => "https://github.com/chef/chef-server.git"
end

group :development, :test do
  gem "chefstyle", git: "https://github.com/chef/chefstyle.git", branch: "master"
end

gem "chef", git: "https://github.com/chef/chef", branch: "tm/inject_log"
gem "ohai", git: "https://github.com/chef/ohai", branch: "tm/inject_log"

if ENV["GEMFILE_MOD"]
  puts "GEMFILE_MOD: #{ENV['GEMFILE_MOD']}"
  instance_eval(ENV["GEMFILE_MOD"])
end
