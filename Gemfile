source "https://rubygems.org"

def ar_version
  version = ENV["AR_VERSION"] || 'default'

  case version
  when 'default'
    ">= 2.0.0"
  when 'master'
    {github: 'rails/rails'}
  else
    "~> #{version}.0"
  end
end

gem 'activerecord', ar_version

group :development, :test do
  gem 'spec'
  gem 'rspec', '>= 1.2.9'
  gem 'rake'
end

group :development do
  gem 'jeweler'
  gem 'appraisal', :github => 'thoughtbot/appraisal'
  gem 'simplecov', :require => false
end
