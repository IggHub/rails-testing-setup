# Rails setup for TDD using RSpec and Capybara

1. `rails new myApp -database=postgresql -T`
2. Inside `:development, :test` add:

```
gem 'rspec-rails', '~> 3.7'
gem 'database_cleaner', '~> 1.6', '>= 1.6.2'
gem 'factory_bot', '~> 4.8', '>= 4.8.2'
```

3. Inside `:test` add:

```
gem 'capybara', '~> 2.17'
gem 'selenium-webdriver', '~> 3.8'
gem 'shoulda-matchers', '~> 3.1', '>= 3.1.2'
```

4. Install rspec: `rails generate rspec:install` (if you receive an error, follow https://stackoverflow.com/questions/39542169/rails-5-could-not-find-generator-rspecinstall)
