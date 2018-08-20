source "https://rubygems.org"

gem 'marc'
gem 'rspec'
gem 'traject'
gem 'library_stdnums'

#Check if we are using jruby and store.
is_jruby = RUBY_ENGINE == 'jruby'
if is_jruby
  gem 'traject-marc4j_reader'
else
  gem 'byebug'
end
