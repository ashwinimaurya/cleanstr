# cleanstr
Python Package for Cleaning Strings

PyPI: https://test.pypi.org/project/cleanstr/

Usage:

!pip install cleanstr

from cleanstr import Functions

F=Functions()

names=['John','albertsons','***shit**', 'bro', 'violently']

F=Functions.cleanupName()

for name in names:
    if F.is_valid_name(name):
        print(f"'{name}' is valid name.\n")
    else:
        print(f"'{name}' is NOT valid name!\n")


Output:

'John' is valid name.

'albertsons' is NOT valid name!

'***shit**' is NOT valid name!

'bro' is NOT valid name!

'violently' is NOT valid name!
