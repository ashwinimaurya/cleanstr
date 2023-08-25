# cleanstr
Python Package for Cleaning Strings

PyPI: [https://test.pypi.org/project/cleanstr/](https://pypi.org/project/cleanstr/)

Usage:

!pip install cleanstr

from cleanstr import Functions

F=Functions()

## Name Cleaning. 

#### The code checks for name validity such as against abusive words, common pronouns, adjectives, common slang words. (to be updated more later :))

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
