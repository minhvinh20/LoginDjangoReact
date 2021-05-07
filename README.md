# Guideline to run project
# For Docker Env
docker-compose -f docker-compose-dev.yml up --build
# For Local Env
### Create env python for project
cd backend

virtualenv venv

source venv/bin/activate

pip install -r requirements.txt
### runserver
cd server

python manage.py runserver

## Run FrontEnd

cd frontend

npm install

npm start
