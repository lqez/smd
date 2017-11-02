## slmd
[![Build Status](https://travis-ci.org/lqez/slmd.svg?branch=master)](https://travis-ci.org/lqez/slmd)
[![codecov](https://codecov.io/gh/lqez/slmd/branch/master/graph/badge.svg)](https://codecov.io/gh/lqez/slmd)

Sort lists in Markdown

### Installation

```
$ pip install slmd
```

### Usage

```
$ slmd <infile> [outfile] [-s ORDER_BY ...]

- If you want to sort only the first depth by ascending order,
$ slmd some.md -s 1

- If you want to sort only the second depth by descending order,
$ slmd some.md -s 0 -1

- Save the result as a file
$ slmd src.md out.md
```

or use it in Python code

```
from slmd import sort_string

result = sort_string(some_markdown_string)
```


### Exit code

 - 0
     - Nothing to sort.
 - 1
     - I sorted something.


### Why do I have to use this?

I made it for managing `awesome-blahblah` list. And you can use it when you want to check list items are ordered properly.

### License
MIT
