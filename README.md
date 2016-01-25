
quaint-yaml
===========

YAML support for the `data` and `include` macros in
[Quaint](http://breuleux.github.io/quaint).


## Install

    quaint --setup yaml


## Usage

This will make a table with two rows and two columns:

```quaint
plugins :: yaml

format table :: data yaml ::
  -
    - one
    - two
  -
    - un
    - deux
```

And this will import YAML from a file:

**data.yaml**

```yaml
a: 1
b: 7
```

**file.q**

```quaint
include :: data.yaml

{a} + {b} == 8
```



## Options

There are no options at the moment.
