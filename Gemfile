source "https://rubygems.org"

ruby RUBY_VERSION

DECIDIM_VERSION = { git: 'https://github.com/decidim/decidim.git', branch: '0.19-stable' }

gem 'decidim', DECIDIM_VERSION
gem 'decidim-file_authorization_handler', git: "https://github.com/MarsBased/decidim-file_authorization_handler.git"
# gem 'decidim-consultations', "~> #{DECIDIM_VERSION}"

gem 'delayed_job_active_record'
gem 'daemons'
gem "whenever", require: false

gem 'puma', '~> 3.12'
gem 'uglifier', '>= 4.0.0'
gem 'faker', '~> 1.8.4'

gem 'figaro', '>= 1.1.1'

# Force gem version to fix:
# undefined method `polymorphic?' for ActiveRecord::Reflection::PolymorphicReflection
# See: https://github.com/activerecord-hackery/ransack/issues/1039
gem 'ransack', '2.1.1'

group :development, :test do
  gem 'byebug', platform: :mri
  gem 'decidim-dev', DECIDIM_VERSION
end

group :development do
  gem 'web-console'
  gem 'listen', '~> 3.1.0'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'letter_opener_web', '~> 1.3.0'

  gem 'better_errors', '>= 2.3.0'
  gem 'binding_of_caller'
end
