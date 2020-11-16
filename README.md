# Memestra Testcase

**versions:**
```
beniget                       0.3.0
gast                          0.4.0
memestra                      0.0.7
nbconvert                     5.6.0
nbformat                      4.4.0
```

When using a deprecated class `Test` that was imported, and then re-exported by `testmodule`, memestra does not recognized the use of deprecated code.

**output:**
```
$ memestra --recursive test.py
```

**expected output:**
```
$ memestra --recursive test.py
testimport.Test used at test.py:3:5 This is deprecated
```