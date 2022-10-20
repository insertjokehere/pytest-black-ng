pytest-black-ng
============

A pytest plugin to enable format checking with [black](https://github.com/ambv/black).

This is a fork of the original [pytest-black](https://github.com/shopkeep/pytest-black) plugin by ShopKeep Inc to provide an up-to-date version of this plugin.


Requirements
------------

* [pytest](https://docs.pytest.org/en/latest/)
* [black](https://github.com/ambv/black)

There is a minimum requirement of black 22.1.0 or later.

Installation
------------

```
$ pip install pytest-black-ng
```


Usage
-----

To run pytest with formatting checks provided by black:

```
$ pytest --black
```

The plugin will output a diff of suggested formatting changes (if any exist). Changes will _not_ be applied automatically.


Configuration
-------------

You can override default black configuration options by placing a `pyproject.toml` file in your project directory. See example configuration [here](https://github.com/ambv/black/blob/master/pyproject.toml).



Testing
-------

To run the tests against a selection of Python interpreters:

```
$ tox
```

To run against a specific interpreter (e.g. Python 3.6):

```
$ tox -e py36
```

The `tox.ini` file in the root of this repository is used to configure the test environment.


License
-------

Distributed under the terms of the `MIT` license, `pytest-black-ng` is free and open source software


Issues
------

If you encounter any problems, please [file an issue](https://github.com/insertjokehere/pytest-black-ng/issues) along with a detailed description.
