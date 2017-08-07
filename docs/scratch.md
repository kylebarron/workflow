

## File Purposes:

00preamble:
    - Define globals
        - data folder?
        - out folder?
    - any programs that are only for this project that are used in almost every file, but not used in any other project
01get
    - rename variables to a standardized format
    - "id_" should be the prefix for any/all variables needed to uniquely identify observations in the data

#### Use git for every project

- Put everything other than data/ in Git in general. 
- Don't add any large binary files, but do add small binary files like PDFs, especially ones that take a lot of computation time to generate. This way, you can go back to a previous commit and view those pdfs without needing to recompile the project.

#### Keep a folder self-contained

- **Never** use absolute paths in a project. 
- Use symlinks profusely, so that paths can look cleaner, but always have them be relative paths

This is so that your folder can easily move around, and everything will still work. If you use absolute paths in a project, then if you ever move that folder to any other location, everything will break.

Whenever you find a great idea from stack exchange, put the link in a comment next to the code. (Stack exchange probably isn't going to go under soon). 

#### Variable naming:
Snake case
camel case, etc
"Two hard things in CS, naming things and ..."

#### Name data folders by unit of observation