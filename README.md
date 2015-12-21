# rubyonrails-pinboard
Ruby on Rails - Pinboard

Following this example video

https://www.youtube.com/watch?v=abcnfFS_DS8

To install gems when the network blocks access to rubygems for direct insatllation through the Gemfile, alternatively you can download each required gem here

https://rubygems.org/gems

Save the downloaded gem file to a temporary directory, then from within this temporary directory run the following command

gem install --force --local *.gem

This will install the gems.

NOTE: some gems may be dependent on other gems (so you will need to download them as well)

Always run the following command after this

bundle install

This will register the gems in your application.

Then restart the Ruby server by typing

rails server

NOTE: 'devise' gem, https://github.com/plataformatec/devise

This gem requires that you go through its documentation, for it to work:

=========================== devise setup =====================================

Some setup you must do manually if you haven't yet:

  1. Ensure you have defined default url options in your environments files. Here
     is an example of default_url_options appropriate for a development environment
     in config/environments/development.rb:

       config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }

     In production, :host should be set to the actual host of your application.

  2. Ensure you have defined root_url to *something* in your config/routes.rb.
     For example:

       root to: "home#index"

  3. Ensure you have flash messages in app/views/layouts/application.html.erb.
     For example:

       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p>

  4. If you are deploying on Heroku with Rails 3.2 only, you may want to set:

       config.assets.initialize_on_precompile = false

     On config/application.rb forcing your application to not access the DB
     or load models when precompiling your assets.

  5. You can copy Devise views (for customization) to your app by running:

       rails g devise:views

===============================================================================

NOTE: 'paperclip' gem, https://github.com/thoughtbot/paperclip

This gem requires that you go through its documentation, for it to work