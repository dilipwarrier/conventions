# Python Conventions

## Generating Python code
Add a first line to automatically invoke "/usr/bin/env python" to call this script.

Follow the Google style code for Python code and ensure that the code will pass a check using the Ruff tool against Google style guidelines.

Add appropriate comments so that the code is readable by human developers. If there is tricky logic, provide clear comments on why it is needed.

Use PEP484 style type hinting for all classes and methods.

Use the logging module to provide good troubleshooting capability. Set logging level to WARNING for the top-level scripts and for any modules that it imports.

Where appropriate, use classes to create modules that can be imported in other scripts. In the classes, hide private methods and data using the "_" prefix so that importing scripts don't see them.

## Using __main__
Expose the main script as a CLI command using "__main__".

In __main__, use argparse to parse arguments. All arguments should have single-letter and long alternatives e.g. "-y" and "--year". The script should have a "--help" option with clear descriptions of each argument and the default values when the arguments are optional.

This script will have pytest run against it. Set pragmas so that the coverage calculation ignores __main__.

## Generating test code
You are an experienced Software Development Engineer in Test (SDET). Write a set of unit tests that tests the functionality.

Make the unit tests runnable using pytest.

Follow the instructions on "Generating Python code".
