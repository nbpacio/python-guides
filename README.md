# Python Programming Guide

List of guides for Python Programming

## PRE Program

### Create Local Repository Folder:

'''powershell
mkdir folder_name
'''

'''powershell
cd folder_name
'''

### Create Virtual Environment:

'''powershell
python -m venv .venv
'''

Windows:

'''powershell
./.venv/Scripts/Activate.ps1

Linux:

'''bash
source .venv/bin/activate
...


### Create File/Scripts:

Windows:

'''powershell
echo This is a sample file. > test.xt 
'''
 Note: use >> to append

Linux:

'''bash
touch file.txt
'''

### Initialize Git (OUTSIDE .ENV):

'''powershell
git init
'''

### Create Git Ignore:

'''powershell
# create-gitignore.ps1

echo ".venv" > .gitignore
echo "venv" >> .gitignore
echo "env" >> .gitignore
echo ".env" >> .gitignore
'''

or place this into the .gitignore file:

'''powershell
# Virtual environments
.venv
venv/
env/
ENV/

# Environment variables
.env
*.env
'''


### Install Modules (Inside ENV):

'''powershell
pip install python-dotenv
pip install openai
'''

### Create Requirements List (requirements.txt):

'''powershell
python-dotenv>=1.0.0
openai>=1.0.0
'''












