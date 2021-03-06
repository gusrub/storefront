# Sports Store

A sports online store demo where the challenge was to NOT use any CSS framework. Written in rails. 

## Installation

Run the following, make sure you have the header libraries of native components because postgres and nokogiri for instance require those:

`bundle install`

## Configuration

We are using [dotenv](https://github.com/bkeepers/dotenv) for configuration of the application. Basically you have `.env` files, one per environment if you want like `.env.development`, or `.env.test` for testing, if you just have `.env` it will override others.

Take a look at the included `.env.example` file for the required values and change them, then rename the file accordingly to `.env.development` for instance. Note you also need a `.env.test` to run the tests.

## Initialization

After installing everything and setting up the environment make sure you create the database:

`rake db:reset`

And that's it, now you can run it with the usual:

`rails server`

## Testing

Prepare test database:

`RAILS_ENV=test rake db:drop db:create db:migrate`

Run tests:

`RAILS_ENV=test rake test`
