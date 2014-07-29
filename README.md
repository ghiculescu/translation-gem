# gem for [Rails Translation](http://rails.translation.io)

## Description

Add this gem to your [Rails](http://rubyonrails.org) app to translate it with [Rails Translation](http://rails.translation.io).

## Installation

Add the gem to your project's Gemfile :

    gem 'translation'

Then :

* Create a translation project from the UI.
* Copy the initializer into your Rails app (`config/initializers/translation.rb`)

And finish by inititalizing your translation project :

    bundle exec rake translation:init

## Synchronization

To get new translations from Rails Translation and to send new translatable strings, simply run :

    bundle exec rake translation:sync

## Purge

If you need to remove unused keys taking the current branch as reference :

    bundle exec rake translation:purge

Warning : all keys that are not present in the current branch will be **permanently deleted both on Rails Translation and in your app**.

## Tests

    bundle
    bundle exec rspec

## Credits

This plugin in released under MIT license by Aurélien Malisart and Michaël Hoste (see MIT-LICENSE
file).

(c) http://rails.translation.io