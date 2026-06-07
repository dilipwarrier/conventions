# Generic Coding Conventions

This document covers generic coding conventions that are relevant to all
programming languages.

For language-specific conventions (e.g. Python, Java), refer to the
other markdown files in this folder.

Code should be easily readable and understandable by humans. Use
appropriate comments so that the code is readable by human
developers. Use comments to explain the "why", not the "how". If there
is tricky logic, provide clear comments on why it is needed.

Keep functions and methods small and focused on a single
responsibility.

Use the "Don't Repeat Yourself" (DRY) principle. When code can be
encapsulated into a method that is called in multiple places, do
so. Similarly, if one constant can be derived from another, for
example, one string can use another string as a prefix, then prefer
that rather than repeating the characters in the string in both
places.

Keep your commits and pull requests small. Commit and push frequently
to development branches.
