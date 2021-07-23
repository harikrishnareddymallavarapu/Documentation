Reference : https://sphinx-intro-tutorial.readthedocs.io/en/latest/sphinx_first_steps.html
https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github

## Getting Started With Sphinx and Restructured Text
====================================================

1. Create a new directory (docs) in the project
```
$ mkdir docs
```
2. Within in the docs directory activate the python environent
```
$ cd docs
[../docs]$ python3 -m venv .env
[../docs]$ source .env/bin/activate
```
3. Install Sphinx 3.5.4 in the virtual environment
```
(.env)[../docs]$ python3 -m pip install -U pip Sphinx==3.5.4
```
4. Run sphinx-quickstart and answer the questions
```
(.env)[../docs]$ sphinx-quickstart
```
5. Post answering, we should see the following folders in docs directory
```
/_build/
/_static/
/_templates
conf.py
index.rst
make.bat
Makefile
make.bat
```
6. we can create html documentation using the following syntax. You can notice the HTML file under _build\html  
```
(.env)[../docs]$ make html
```
7. Autobuild sphinx documentation
```
(.env)[../docs]$ sphinx-autobuild . ./_build/html

```
