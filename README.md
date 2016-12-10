XML cleaner
-----------

Word and sentence tokenization in Python. Tested in Python `3.4.3` and `2.7.12`.

[![PyPI version](https://badge.fury.io/py/xml-cleaner.svg)](https://badge.fury.io/py/xml-cleaner)
[![Build Status](https://travis-ci.org/jonathanraiman/xml_cleaner.svg?branch=master)](https://travis-ci.org/jonathanraiman/xml_cleaner)
![Jonathan Raiman, author](https://img.shields.io/badge/Author-Jonathan%20Raiman%20-blue.svg)

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)


Usage
-----

Use this package to split up strings according to sentence and word boundaries.
For instance, to simply break up strings into tokens:

```
tokenize("Joey was a great sailor.")
#=> ["Joey ", "was ", "a ", "great ", "sailor ", "."]
```

To also detect sentence boundaries:

```
sent_tokenize("Cat sat mat. Cat's named Cool.", keep_whitespace=True)
#=> [["Cat ", "sat ", "mat", ". "], ["Cat ", "'s ", "named ", "Cool", "."]]
```

`sent_tokenize` can keep the whitespace as-is with the flags `keep_whitespace=True` and `normalize_ascii=False`.

Installation
------------

```
pip3 install xml_cleaner
```

Testing
-------

Run `nose2`.
