## Welcome to our group!

This site contains some basic information about our group and about how we do things.

---

## Getting started

- We use GitHub for VC. Please make __absolutely__ sure that no personally identifiable data is __ever__ uploaded to GitHub.
- We use Slack for collaboration. Please ask for an invite on your first day.
---

## Python Styleguide

Please stick to the [Google style guide](http://google.github.io/styleguide/pyguide.html) in general with some changes here or there:

- We use 2 spaces for indentation (__don't use tabs__ or rebind them to 2 spaces in your editor)

- We use the [black](https://black.readthedocs.io/en/stable/) autoformatter.

- We use [type annotations](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html) and a static type checker like [mypy](http://mypy-lang.org).

- We use [pytest](https://docs.pytest.org/en/latest/) for testing.

- Please use google-style docstrings with the following format:

```python
def somefunc(x:Any)->None:
  """General description goes here.

  Args:
    argument1: Description of argument 1. Don't include the 
               type here as it is annotated above

  Returns:
    Description of the return value. 
    Don't include the type as it is annotated above.

  Raises:
    SomeErrorType: Cause of the exception.
      
  Logs:
    If you have logging enabled (which we recommend), 
    explain what gets logged.
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

- We aim for reproducible, reusable and multi-purpose code. Please don't use Jupyter for everything but refactor your experiments into a library in the following way:
 - A notebooks section which mirrors your experimental strategy. Make _**absolutely**_ sure that you don't have cells in there which contain personal information or any other sensitive data.
 - A `src` or `scripts` folder which contains one `.py` module per experiment and/or figure with descriptive naming.
 - Appropriate tests

- Please make sure you include an `environment.yml` file or at the very least a `requirements.txt` file.
- Create one repository per project. Make use of issues and PRs to update code. Use the wikis and project boards.

- Please stick to the following project template:

```
-Top-level directory
|
|-data_directory
|
|-environment.yml
|
|-notebooks_directory
|----00_EDA.ipynb
|----01_Experiment_1.ipynb
|----...
|-scripts_directory
|----__init__.py
|----module1.py
|----module2.py
|-tests_directory
|----__init__.py
|----test_module1.py
|----test_module2.py
```
---

## Conda

Please use [conda environments](https://conda.io/en/latest/miniconda.html) as much as possible. Create a new env for each project and please upload the `environment.yml` file to VC so that people can easily re-create your experiments. 

---

## Writing

- If you want to use plain text or markdown (which is our preferred solution), create a `manuscripts` folder in your repository and place your text there, either as chapters or as sections (Introduction, Material etc.).

- If you want to use LaTeX, we prefer to use [Overleaf](https://www.overleaf.com)

- If you want to use a word processor, please use the following style:
  - Arial 14 pts. for Titles
  - Arial 12 pts. for paragraph headings
  - Arial 11 pts. for the text
  - 1.5 pt. line spacing
  - _italics_ for latin terms or standard terms (e.g. _quasi-mesenchymal_)
  - Don't use bold or underlined
  - Colour references to include later or anything else yellow
  
- For monospaced text, please use [Fira Code](https://github.com/tonsky/FiraCode). It's a great font for your editor, too!





