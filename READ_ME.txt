Hey Jack. You never remember this shit so here you go: #HOWTO

this is a project done following Tech with Tims video @ 
https://www.youtube.com/watch?v=c-QsfbznSXI&list=PL4CRa1ZaEul-qmrVVBoGAjdWJ37ndP3H1&index=5&ab_channel=TechWithTim 

the database is connected to Chromeo as a test account so will fail if chromeo times out. to update this backend/backend/settings/DATABASES#NOTE you can set it back to the sqlite one
your chromeo account details are in the env directory

tips for using Django + React to get the servers running:
# create a new venv (for first time only)
python -m venv env
.\env\Scripts\Activate.ps1

# create a requirements.txt file in project root directory copy all requirements on \n (first time only)
pip install -r requirements.txt

### BACKEND ###
# makesure you are in venv (env)
    cd FULLSTACK
    .\env\Scripts\Activate.ps1

# load changes to backend/databases
    python manage.py makemigrations

# push changes
    python manage.py migrate

# run server
    python manage.py runserver

### FRONTEND ###
# install all dependencies added
npm install

#run frontend server
npm run dev

### GITHUB ###
( do this inside your (env) project root (FULLSTACK) )

## remove an init from the wrong location (navigate to the parent directory)
# Remove the .git directory
Remove-Item -Force -Recurse .git

# make a new github repository 
    git init

# add all files to git holding
    git add .

# commit 
    git commit -m "first-commit"

# convert branch from MASTER to MAIN
    git branch -M main

# create a new repository on GitHub and get the url (paste url down here)
    git remote add origin https://github.com/09heatherj/notes-full-stack-twt.git

# push to repository
    git push -u origin main
