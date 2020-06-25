This is a fork of [topia.termextract](https://github.com/turian/topia.termextract) to make this library compatible with Python 3

Fixes : 
- The `interface.implements()` from zopia is deprecated and should now use the `@implementer` annotation
- Fix as the the library would not run under Windows since the Timeout decorator was using SIGTERM of the signal module which is not available under Windows
- Fix the uses of ulrlib2 which has changed in Python3
- Replace [re2](https://pypi.org/project/re2/) which is not Python 3 compatitable with [regex](https://pypi.org/project/regex/)

To install, simple add the following to your `requirements.txt` file
```
git+git://github.com/FlyingCowMooMoo/topia.termextract.git
```

or to install using `pip` run the following:  
```
pip install git+git://github.com/FlyingCowMooMoo/topia.termextract.git
```
