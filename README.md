# Memestra Testcase

**versions:**
```
beniget                       0.3.0
gast                          0.4.0
memestra                      0.0.6
nbconvert                     5.6.0
nbformat                      4.4.0
```

**output:**
```
$ memestra --recursive test.py
testimport.Test used at test.py:3:5
```

**expected output:**
```
$ memestra --recursive test.py
testimport.Test used at test.py:3:5 This is deprecated
```