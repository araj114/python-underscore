Python Underscore
=================

A python port of Underscore.js.

Current Status
--------------

Unfinished.

How to Use
----------

    from underscore import Underscore
    _ = Underscore()

    # functional style
    _.each([1,2,3,4,5], lambda x: return x + 1)

    # object-oriented style
    _([1,2,3,4,5,6]).each(lambda x: return x + 1)


Methods
-------

It's currently under development at the moment.

###each

    _.each(sequence, function)

Tested to support sequences (but not dictionaries yet).

    _.each([1,2,3,4,5], lambda x: x + 1)
    > [2,3,4,5,6]
    
###mixin

    mixin(<dictionary_of_methods>)

A method for extending underscore.

    def util_method(self, x, y):
      return x + y

    _.mixin({
      'my_method': util_method
    })

    _.my_method(1,2)
    > 3

Do note that in each method, the explicit 'self' argument has
to be there.

Contributing
------------

Just fork the project and submit a pull request.

It is best to write a test for each feature.


Author
------

You can contact me via my email: me@jpanganiban.com
