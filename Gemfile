source ENV['GEM_SOURCE'] || 'https://rubygems.org'
puppetversion = ENV.key?('PUPPET_VERSION') ? ENV['PUPPET_VERSION'] : ['>= 3.3']

group :test do
  gem 'coveralls'
  gem 'facter', '>= 1.7.0'
  gem 'git', '1.3.0'
  gem 'httparty'
  gem 'metadata-json-lint'
  gem 'puppet', puppetversion
  gem 'puppet-blacksmith'
  gem 'puppet-lint', '>= 1.0.0'
  gem 'puppet-strings'
  gem 'puppetlabs_spec_helper', '>= 1.0.0'
  gem 'rspec-puppet'
  gem 'rspec-puppet-utils'
  gem 'rspec_junit_formatter'
end

group :acceptance do
  gem 'beaker'
  gem 'beaker-puppet_install_helper'
  gem 'beaker-rspec'
  gem 'pry'
end

# rspec must be v2 for ruby 1.8.7
if RUBY_VERSION >= '1.8.7' && RUBY_VERSION < '1.9'
  gem 'rake', '~> 10.0'
  gem 'rspec', '~> 2.0'
else
  # rubocop requires ruby >= 1.9
  gem 'rubocop'
end
