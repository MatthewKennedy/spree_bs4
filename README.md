# SpreeBs4

Adds Bootstrap 4 into the frontend of Spree. This extension is intended to be used after spree_remove_bs3 gem has been installed.

Please be aware that you will need to pick through your Spree frontend view files replacing the old Bootstrap 3 classes with the relevant Boostrap 4 classes.

## Installation

1. Add these lines to the bottom of your Gemfile:
  ```ruby
  gem 'spree_remove_bs3', github: 'matthewkennedy/spree_remove_bs3'
  gem 'spree_bs4', github: 'matthewkennedy/spree_bs4'
  ```

2. Install the gem using Bundler:
  ```ruby
  bundle install
  ```

3. Copy & run the following commands in order
  ```ruby
  bundle exec rails g spree_remove_bs3:install
  bundle exec rails g spree_bs4:install
  ```

4. Restart your server

  If your server was running, restart it so that it can find the assets properly.

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_bs4/factories'
```


## Contributing

If you'd like to contribute, please take a look at the
[instructions](CONTRIBUTING.md) for installing dependencies and crafting a good
pull request.

Copyright (c) 2018 [name of extension creator], released under the New BSD License
