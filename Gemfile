source 'https://rubygems.org'
ruby '2.3.3'


# Workaround https://github.com/bundler/bundler/issues/3324 until Bundler 2.0
git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end


#
# Server
#

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.0.2'
# Use Postgres as the database in all environments
gem 'pg'
# Use Puma as the app server
gem 'puma', '~> 3.0'
# Load environment variables from config/application.yml
gem 'figaro'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
# gem 'redis', '~> 3.0'
# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

#
# Assets
#

# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Fixes https://github.com/rails/coffee-rails/issues/87
gem 'coffee-script-source', '1.8.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.2'
# Use browserify to process client JS and gain modules & ES6 features
gem 'browserify-rails'
# See https://github.com/rails/execjs#readme for more supported runtimes
gem 'therubyracer', platforms: :ruby

#
# Dev Tools
#

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: [:mri, :x64_mingw]
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'web-console', '>= 3.3.0'

  # Add a profiling helper to every page
  # gem 'rack-mini-profiler'

  # For memory profiling (requires Ruby MRI 2.1+)
  # gem 'memory_profiler', platforms: [:mri, :x64_mingw]

  # For call-stack profiling flamegraphs (requires Ruby MRI 2.0.0+)
  # gem 'flamegraph', platform: :mri
  # gem 'stackprof', platform: :mri
  # gem 'fast_stack', platform: :mri
end
