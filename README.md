## Welcome to our group!

This site contains some basic information about our group and about how we do things.

---

## Getting started

- We use GitHub for VC. Please make __absolutely__ sure that no personally identifiable data is __ever__ uploaded to GitHub.

---

## Python Styleguide

Please stick to the [Google style guide](http://google.github.io/styleguide/pyguide.html) in general with some changes here or there:

- We use 2 spaces for indentation (__don't use tabs__ or rebind them to 2 spaces in your editor)

- We use the [black](https://black.readthedocs.io/en/stable/) autoformatter.

- We use [type annotations](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html) and a static type checker like [mypy](http://mypy-lang.org).

- We use [pytest](https://docs.pytest.org/en/latest/) for testing.

- Please use google-style docstrings with the following format:

```python
def somefunc(x:Any)->:
    """General description goes here.

    Args:
      argument1: Description of argument 1. Don't include the type here as it is
                 annotated above

    Returns:
      Description of the return value. Don't include the type as it is annotated above.

    Raises:
      SomeErrorType: Cause of the exception.
      
    Logs:
      If you have logging enabled (which we recommend), explain what gets logged.
    """
```

- Adhere to PEP8. Avoid things like:

```python
def myfunc(x) : return x
```

```python
if self.store.stretch_dir==0: x = stretch_cv(x, self.store.stretch, 0)
else:                         x = stretch_cv(x, 0, self.store.stretch)
```
In general, avoid every single recommendation on [this site](https://docs.fast.ai/dev/style.html#jeremys-notes-on-fastai-coding-style).

---

## Jupyter Notebooks

- We use JupyterLab, not the old notebook interface anymore

- We aim for production-ready code. Please don't use Jupyter for everything but refactor your experiments into a library.

- If you use Jupyter, please stick to the following project template:

-Top-level directory
|
|-data_directory
|
|-notebooks_directory
|----00_EDA.ipynb
|----01_Experiment_1.ipynb
|----...
|-scripts_directory
|----\_\_init__.py
|----module1.py
|----module2.py
|-tests
|----\_\_init__.py
|----test_module1.py
|----test_module2.py

---

## Writing

- If you want to use LaTeX, please use [Overleaf](https://www.overleaf.com)

- If you want to use a word processor, please use the following style:
  - Arial 14 pts. for Titles
  - Arial 12 pts. for paragraph headings
  - Arial 11 pts. for the text
  - 1.5 pt. line spacing
  - _italics_ for latin terms or standard terms (e.g. _quasi-mesenchymal_)
  - don't use bold or underlined
  - colour references to include later or anything else yellow
  
- For monospaced text, please use [Fira Code](https://github.com/tonsky/FiraCode). It's a great font for your editor, too!





