# Intro To Git

Git ReadMe files and Juypiters text is written in [Markdown](https://www.markdownguide.org/cheat-sheet/), a simple markup language

### Main git Commands
- `git add` - specify which files are to be added to the repository, everything in file can be specified with "."
- `git commit -m` "commit message" - commits the changes to the local git system
- `git push` - pushes the changes to the cloud hoested Version Control on github
- `git clone repoLink` - creates a local copy of the respository in the called location

A standard set of commands when updating a repository after work is:
```bash
  git add .
  git commit -m "specify changes made"
  git push
```

## Python best Practices
### Using a Virtual Enviroment 
The use of a virtual enviroment in python is good for encapluating code, it allows you to store the libraries used with the code so that when a project is run on another computer you dont need to reinstall all used libraries.

To create a virtual enviroment navigate to the project directory and run the terminal command `python3 venv enviromentName`

To activate the virual enviroment naviagate to the home directory and run the terminal command `enviromentName/Scripts/activate`


## Jutpiter Notebook
### Finding Datasets
- [Kaggle](https://www.kaggle.com/datasets)
