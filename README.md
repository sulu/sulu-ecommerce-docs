# Sulu Ecommerce Documentation

This is the Sulu eCommerce Documentation for Developers. Clone it to your local
mashine or read the [online docs](http://sulu-ecommerce-docs.readthedocs.org/en/latest/).

## Requirements

Make sure these requirements are installed:

* python2.7

To install the requirements above you could use fancy brew:

```
brew install python
```

## Installation

#### Buildout

The buildout script is a very helpful tool to automatically download and install
all dependencies to your local environment. It also generates scripts for your daily
use.

Bootstrap with python 2.7:

```
/opt/local/bin/python2.7 bootstrap.py
```

Now you can run buildout:

```
bin/buildout -N
```

## Sphinx

If you have changed the docs run this task to compile your text files to html:

```
bin/make-docs
```

View your local docs in your browser:

```
bin/docs
```
