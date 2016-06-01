# turbolinks-source-gem

Quickly add Turbolinks to your Rails app without the overhead of coffeescript and building the compiled JS from source.

## Gemfile

```ruby
gem 'turbolinks-source', '~>5.0.0.beta5'
```

## Rails Configuration

Give Rails an additional path to find assets in:

```ruby
# config/initializers/assets.rb

Rails.application.config.assets.paths << Turbolinks::Source.asset_path
```

## Asset Inclusion

Include Turbolinks in the list of scripts going down to the client:

```javascript
// app/assets/javascripts/application.js

//= require jquery
//= require turbolinks
// ...your other includes here...
```
    
Enjoy!
