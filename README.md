# ModBootstrap

Welcome to your new gem! In this directory, you'll find the files you need to be able to package up your Ruby library into a gem. Put your Ruby code in the file `lib/mod_bootstrap`. To experiment with that code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'jquery-rails'
gem 'bootstrap-sass'
gem 'mod_bootstrap'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jquery-rails
    $ gem install bootstrap-sass
    $ gem install mod_bootstrap

## Usage

Import Bootstrap styles in `app/assets/stylesheets/application.scss`:

```scss
// "bootstrap-sprockets" must be imported before "bootstrap" and "bootstrap/variables"
@import "bootstrap-sprockets";
@import "bootstrap";
@import "mod_bootstrap";
```

Require Bootstrap Javascripts in `app/assets/javascripts/application.js`:

```js
//= require jquery
//= require bootstrap-sprockets
```

`bootstrap-sprockets` and `bootstrap` [should not both be included](https://github.com/twbs/bootstrap-sass/issues/829#issuecomment-75153827) in `application.js`.

`bootstrap-sprockets` provides individual Bootstrap Javascript files (`alert.js` or `dropdown.js`, for example), while
`bootstrap` provides a concatenated file containing all Bootstrap Javascripts.
## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/mod_bootstrap.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
