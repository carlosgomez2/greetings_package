# Package example

This is an example to create a package and use it accross multiple apps

1. Install `pip3 install setuptools` to build greetings_package from `setup.py`
2. Then execute `python3 setup.py sdist` from root directory
3. Then install the package `pip3 install .`
4. Use the package in another project calling `greetings_module==0.0.1` and installing requirements.txt with pip3 if the package is published on pypi or use file:///route-to-package/package.tar.gz in requirements
5. Use it

```python
from greetings_package.greetings_module import greetings

print(greetings()) # You should se a greeting
```
