# Capybara

Add `rspec-rails` and `capybara` to '''both''' the `:development` and `:test` groups in the Gemfile

```
group :development, :test do
  gem 'rspec-rails', '~> 3.0.0'
  gem 'capybara', '~> 2.3.0'
end
```

Initialize the `spec/` directory (where specs will reside) with:

```
rails generate rspec:install
```

Create the `features` folder in `spec` folder, write the first acceptance test.

## Resources

- https://github.com/rspec/rspec-rails
- https://github.com/jnicklas/capybara
- [Warning message](https://github.com/rspec/rspec-rails/issues/1103)