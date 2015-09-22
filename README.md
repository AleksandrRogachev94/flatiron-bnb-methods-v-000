# Flatiron-BnB: Methods

In the previous iteration, we built out our model associations and migrated our database. Now we're going to work on building useful methods (class and instance) for rendering data and our own validations. We're doing this to follow the principle that our controllers should be skinny, our models fat, so therefore our views have very little logic in them.

## Instructions

There are many methods and validations and callbacks to build! They will be challenging.

1. Work together.
2. Go slow.
3. Read the resources.
4. Get the tests to pass.

## About Validations

Validations "allow you to declaratively define valid states for your model objects. The validation methods hook into the life cycle of an Active Record model object and are able to inspect the object to determine whether certain attributes are set, have values in a given range, or pass any other logical hurdles that you specify." (The Rails 4 Way, pg 241)

Custom validation methods should always be `private`, so they can't be called from code outside of the model.

## About Callbacks

Callbacks are ways to attach methods/behavior to different points of a model's life cycle, like before saving and before destroying.

Methods declared as callbacks should always be `private`, so they can't be called from code outside of the model.


## Super Bonus

Instead of creating instance methods `hosts` and `guests`, try to use Active Record associations. The same tests should pass.

## Resources
* [About Private Methods](http://stackoverflow.com/a/4293330/2890716)

* [AR Validations](http://guides.rubyonrails.org/active_record_validations.html)

* [Rails Callbacks](http://api.rubyonrails.org/classes/ActiveRecord/Callbacks.html)
* [Rails 4 Way: Validations](http://beta-library.herokuapp.com/books/the-rails-4-way#page=247)
* [Rails 4 Way: Callbacks](http://beta-library.herokuapp.com/books/the-rails-4-way#page=273)
