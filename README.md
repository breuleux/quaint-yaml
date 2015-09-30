
quaint-yaml
===========

YAML support for the `include` and `format` macros in
[Quaint](http://breuleux.github.io/quaint).

This will make a table with two rows and two columns:

```quaint
plugins :: yaml

format yaml:table
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

```quaint
plugins :: yaml javascript

include :: data.yaml

{a + b} == 8
```



## Options

There are no options at the moment.
