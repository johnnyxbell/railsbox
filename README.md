# Rails Box

[![Build Status](https://travis-ci.org/joshfng/railsbox.svg?branch=master)](https://travis-ci.org/joshfng/railsbox)

Vagrant box provisioned Ruby on Rails applications. Built using [railsbox-packer](https://github.com/joshfng/railsbox-packer). You can find the box hosted on Atlas [here](https://atlas.hashicorp.com/joshfng/boxes/railsbox/)

Includes:
 - Ubuntu 18.04 LTS
 - Latest stable Ruby (via rbenv)
 - Most current version of Bundler & Rails
 - Postgresql
 - Redis
 - Git
 - Node.js installed via NVM with npm and yarn
 - Chrome and Chromedriver for headless testing

## Getting started

```
cd myrailsproject
curl -O https://raw.githubusercontent.com/joshfng/railsbox/master/Vagrantfile
vagrant up
vagrant ssh

#if you don't already have a rails app
rails new .

bundle
bundle exec rake db:create
bundle exec rake db:migrate
```

## Postgresql
PG is installed and the user `vagrant` has permissions to create databases

## License

MIT

## Credit

Josh Frye @joshfng on GitHub and Twitter
