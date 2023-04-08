---
title: Code Style 🖌️
date: 2023-04-07 23:00:00 +200
categories: [backend, development]
tags: [backend, code-style]
---

A few rules to follow when writing code for the project.

1. Use `snake_case` for variables and functions.
2. Use `PascalCase` for classes.
3. Use code formatters to format your code. Check out Black and Flake8 for python.
4. Use docstrings and typing to document your code. We are automatycally generating Sphinx documentation from docstrings, so make sure to write them for all your functions and classes and files. Format:

   ```python
   """
   This is a module docstring.
   It should describe what the module does.
   """

   def my_function(a: int, b: str) -> dict:
      """
      This is a function docstring.
      It can be multiline and should describe what the function does.

      :param a: This is the first parameter.
      :param b: This is the second parameter.
      :return: This is a description of the return value.
      :raises ValueError: If a is less than 0.
      """
      if a < 0:
         raise ValueError("a must be greater than 0")

      return {"a": a, "b": b}
   ```
