---
title: Python Using Pip
---
We have seen how to use `import` statements to `import` various modules and to use them in our programs. Python itself comes with several built-in modules, but the python community has more to offer.

> Its the modules that makes python so powerful!

Third party modules add so much more functionality to Python. Now we would learn how to install these modules so that we can use those in our programs.

The simplest way is to use `pip`

    pip install <module_name>

If you have used `npm`, then you can think of it as _npm_ of python.

Last time, in <a>`import-statements`</a> wiki we used `requests` module as an example. As it is a third party module we have to install it separately after installing python.

Installing it would be as simple as `pip install requests` . You can even pass various arguments along with it. The one that you'll come across more often is `--upgrade`. You can upgrade a python module by :

    pip install <module_name> --upgrade

For example, to upgrade the requests module to its latest version would be as simple as `pip install requests --upgrade`.

Before using `pip`, you will need to install it (it's quite simple). You can install it from <a href='https://bootstrap.pypa.io/get-pip.py' target='_blank' rel='nofollow'>here</a>

Just click on the link. And save the file as`get-pip.py` _Please don't forget the `.py` extension._ And run it.

An alternative to using pip would be to try <a href='https://bootstrap.pypa.io/ez_setup.py' target='_blank' rel='nofollow'>`easy_install`</a>.

Using `easy_install` is also simple. The syntax is:

    easy_install <module_name>

However, `pip` is more popular than using `easy_install`.

### Adding a project to Pip
Adding your project to Pip is easy:
1. First register an account with PyPi [here](https://pythonhosted.org/an_example_pypi_project/setuptools.html).
2. Then install Twine: `pip install Twine`. Twine is a program that helps you easily upload your project to the PyPi servers.
3. Create a `Setup.py` file as described [here](https://pythonhosted.org/an_example_pypi_project/setuptools.html). The `setup.py` file contains metadata about your project such as version, license, keywords, and contact info.
4. Package your project for upload: `python setup.py sdist`
5. Upload with Twine: `twine upload dist/*`
