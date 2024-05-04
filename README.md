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

#### install all at once
pip install -r requirements.txt
or 
install one by one 

-----
#### to setup git
git config --global user.name 'Navneet Jain'
git config --global user.email 'Navneet######.gmail.com'

--
#### add files to git
git add requirements.txt
#### add all files
git add .
# check git status
git status

-----
#### commit to git
git commit -m "this commit includes requirements.txt"

#### push to main 
git push origin main

#### DONE

### To Create a FLASK Web Application
create app.py
import flask, 
@app.route('/predict_api',methods=['POST'])
def predict_api():
{
}
create a templates folder
html file with in -> <h1> Hello World </h1>

run app.py -> python app.py
application build on web, view on local host
git add.

### Running on POSTMAN
copy local address
provide json data in Body to predict (key-value pairs)
click on send
output achieved

### Prediction from on FRONT END Application
create POST method
@app.route('/predict ',methods=['POST'])
def predict_api():
{
}
create HTML form and predict button, post method
run python file
git add.
git commit -m "The web APP is ready"
git push origin 

### Procfile for Heroku Development
create Procfile
add gunicorn in requirements.txt
within Procfile ->
                  web: gunicorn app:app
#### Login to Heroku desktop
create new app
deployment method -> gitHUB -> account & repo details -> deploy branch
check logs
view application 

#### Deploying the app Using Dockers
create Dockerfile
cmd we've to add 
              FROM python:3.7
              
              COPY . /app
              
              WORKDIR /app
              
              RUN pip install -r requirements.txt
              
              EXPOSE $PORT
              
              CMD gunicorn --workers=4 --bind 0.0.0.0:$PORT app:app create folder   
       
       -> .github
       
       -> workflows -> create file -> main.yaml ( Provide heroku cred ( Heroku api_key, mail, app_name) in this file, by adding it to Action secrets from gitHUB )
       -> git add.
          git commit -m "Dockers is created"
          git push origin 
       

       
       
 




