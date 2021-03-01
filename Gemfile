source "https://rubygems.org"

ruby RUBY_VERSION

DECIDIM_VERSION = { git: 'https://github.com/decidim/decidim.git', branch: 'release/0.21-stable' }

gem 'decidim', DECIDIM_VERSION
gem 'decidim-file_authorization_handler', git: "https://github.com/CodiTramuntana/decidim-file_authorization_handler.git"
# gem 'decidim-consultations', "~> #{DECIDIM_VERSION}"

gem 'delayed_job_active_record'
gem 'daemons'
gem "whenever", require: false

gem 'puma', '< 5'
gem 'rails', '< 6'
gem 'uglifier', '>= 4.0.0'
gem 'faker', '~> 1.8.4'

gem 'figaro', '>= 1.1.1'

group :development, :test do
  gem 'byebug', platform: :mri
  gem 'decidim-dev', DECIDIM_VERSION
end

group :development do
  gem 'listen', '~> 3.1.0'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'letter_opener_web', '~> 1.3.0'

  gem 'better_errors', '>= 2.3.0'
  gem 'binding_of_caller'
end
