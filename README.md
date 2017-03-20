# Tadpole Site
<!---
  TODO: Add code status indicators from CI services. Examples:
  [![Build Status](https://codeship.com/projects/0e40c6d0-4787-0132-ccf4-025f0fbdfe45/status?branch=master)](https://codeship.com/projects/0e40c6d0-4787-0132-ccf4-025f0fbdfe45)
  [![Build Status](https://secure.travis-ci.org/angular-ui/bootstrap.svg)](http://travis-ci.org/angular-ui/bootstrap)
  [![Code Climate](https://codeclimate.com/github/wellbredgrapefruit/asari.png)](https://codeclimate.com/github/wellbredgrapefruit/asari)
  [![Security](https://hakiri.io/github/wellbredgrapefruit/asari/master.svg)](https://hakiri.io/github/wellbredgrapefruit/asari/master)
  [![Test Coverage](https://img.shields.io/coveralls/resque/resque/master.svg)](https://coveralls.io/r/resque/resque)
  [![Inline Doc Coverage](http://inch-ci.org/github/resque/resque.svg)](http://inch-ci.org/github/resque/resque)
-->
A Rails + Vue app that provides Tadpole's website.

## Getting started

### Requirements

To install and use this project you will need:

* Ruby via a version manager like 
  [rvm](https://rvm.io/) or 
  [uru](https://bitbucket.org/jonforums/uru). 
* Node.js via a version manager like 
  [nvm](https://github.com/creationix/nvm) or 
  [nvm-windows](https://github.com/coreybutler/nvm-windows). 
* [Postgres](https://www.postgresql.org/download/).


### Installation

##### Clone the repo into a new directory
Navigate to your web projects directory and use git to clone the project files
into a new directory:
```
git clone https://github.com/path/to/project
```

##### Install Ruby and dependencies
* Use your Ruby version manager to install the version listed in Gemfile.
* `gem install bundler` if not already available for this Ruby
* `bundle install` to install all the packages specified in Gemfile.
* Dependencies can later be updated with `bundle update`.

##### Install Node.js and dependencies
* Use your Node version manager to install the version listed in package.json.
* `npm install` to install all the packages specified in package.json.
* Dependencies can later be updated with `npm update`.


### Configuration
This app loads external configuration from environment variables.

We use Figaro to load this data from `config/application.yml` in development
environments, but this file may contain service keys and thus cannot be 
included via git. Request a copy from a fellow contributor, or roll your own
that provides the required keys listed in `config/initializers/figaro`.


### Database Setup
Use pgAdmin to ensure the database role specified in `application.yml` exists, 
has the correct password, can log in, and can create databases. 

Next, run `rails db:setup` to create the databases, load the schema, and load 
initial data.

The initial data will contain an admin user with name "admin" and password 
"password".


## Running the App
Run `rails server` or simply `rails s`.


## Running Tests
Run `rails test` or simply `rails t`.

This may become more complex as we integrate additional testing frameworks.


## Deploying To Heroku
TODO
