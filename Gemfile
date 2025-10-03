source "http://rubygems.org"

# Specify your gem's dependencies in oauth-plugin.gemspec
gemspec

require 'rbconfig'

if RbConfig::CONFIG['target_os'] =~ /darwin/i
  gem 'rb-fsevent', platforms: :ruby
  gem 'growl'
end

if RbConfig::CONFIG['target_os'] =~ /linux/i
  gem 'rb-inotify', '>= 0.5.1'
  gem 'libnotify',  '~> 0.1.3'
end
