source 'https://rubygems.org'

gemspec

group :test do
  gem 'i18n', require: false
  platform :mri do
    gem 'simplecov', require: false
  end
  gem 'dry-monads', '>= 0.4.0', require: false
  gem 'dry-struct'
end

group :tools do
  gem 'pry-byebug', platform: :mri
  gem 'pry', platform: :jruby

  unless ENV['TRAVIS']
    gem 'mutant', git: 'https://github.com/mbj/mutant'
    gem 'mutant-rspec', git: 'https://github.com/mbj/mutant'
  end
end

group :benchmarks do
  gem 'hotch', platform: :mri
  gem 'activemodel', '~> 5.0.0.rc'
  gem 'actionpack', '~> 5.0.0.rc'
  gem 'benchmark-ips'
  gem 'virtus'
end
