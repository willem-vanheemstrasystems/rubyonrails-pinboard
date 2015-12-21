# rubyonrails-pinboard
Ruby on Rails - Pinboard

Following this example video

https://www.youtube.com/watch?v=abcnfFS_DS8

To install gems when the network blocks access to rubygems for direct insatllation through the Gemfile, alternatively you can download each required gem here

https://rubygems.org/gems

Save the downloaded gem file to a temporary directory, then from within this temporary directory run the following command

gem install --force --local *.gem

This will install the gems.

Always run the following command after this

bundle install

This will register the gems in your application.
