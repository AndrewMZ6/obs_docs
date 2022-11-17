#tests #testing

The thing with assertions is this: when expression inside `assertion` is `true` or `1`  nothing happens
```
assert(true);
assert(1);
```
However in case an expresstion inside `assertion` is `false` or `0` an `Assertion failed` exception is raised
```
assert(false);
assert(0);

Assertion failed.
```

A common usage of assert statement is as follows:
```
assert(Expression)
```
And `Expression` 