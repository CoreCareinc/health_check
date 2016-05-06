source 'https://rubygems.org'

# Specify your gem's dependencies in health_check.gemspec

gemspec

group :development, :test do
  if defined?(JRUBY_VERSION)
    gem 'jruby-openssl'
    gem 'activerecord-jdbcsqlite3-adapter'
  else
    gem 'sqlite3', "~> 1.3.7"
  end
  # run travis-lint to check .travis.yml
  gem 'travis-lint'
  gem 'sidekiq'
  gem 'redis'
  gem 'aws-sdk'
  platforms :ruby_18 do
    # mime-types 2.0 requires Ruby version >= 1.9.2
    gem "mime-types", "< 2.0"
  end

end
