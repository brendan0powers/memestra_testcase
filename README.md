# Memestra Testcase

**versions:**
```
beniget                       0.3.0
gast                          0.4.0
memestra                      0.1.2
```

The module `testimport` has two classes, `Test` and `Foo`.
`Test` is deprecated, `Foo` is not.
When importing using `*`, both classes are marked as deprecated.
When only `Test` should be.
If the classes are imported by name, it works as expected.

**output:**
```
$ memestra test.py
Foo used at test.py:4:5 - This is deprecated
Test used at test.py:3:5 - This is deprecated
```

**expected output:**
```
$ memestra test.py
Test used at test.py:3:5 - This is deprecated
```