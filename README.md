# Freefind Rails

Easy way to use freefind.com search service in your Rails app. You need to create an account at freefind.com first.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'freefind_rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install freefind_rails

Include the javascript into the asset pipeline:
/app/assets/javascripts/application.js

    //= require freefind

## Usage

Add the _freefind_search.html.haml view partial where you want the search input box to appear

    = render partial: 'freefind_search', locals: { freefind_site_id: your-id }

Make sure to pass your freefind site id into the partial as a local variable. This can be done in the parent application using a Rails configuration file.

## Contributing

1. Fork it ( https://github.com/[my-github-username]/freefind_rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
