### Rice crop Disease Prediction

### Softwarers and Tools Requirements

1. [GithubAccount]
2. [HerokuAccount] 
3. [VScodeIDE]
3. [GitCLI] 
(Getting-Started-The-Command-Line)

Create a new environment

...
conda create -p venv python=3.7 -y
or 

python -m venv myenv
pip install pipenv
pipenv shell
...
Add all required software/ Tools in requirements.txt
Add read.me file for info

# install all at once
pip install -r requirements.txt
or 
install one by one 

-----
# to setup git
git config --global user.name 'Navneet Jain'
git config --global user.email 'Navneet######.gmail.com'

--
# add files to git
git add requirements.txt
# add all files
git add .
# check git status
git status

-----
# commit to git
git commit -m "this commit includes requirements.txt"

# push to main 
git push origin main

# DONE
