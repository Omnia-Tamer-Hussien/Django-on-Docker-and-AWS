# Django-on-Docker-and-AWS
A simple python Django web page for cheking if patient data existed on hospital DB or not
# HOW TO RUN THIS PROJECT
Install Python(3.7.6) (Dont Forget to Tick Add to Path while installing Python)

Open Terminal and Execute Following Commands :

`` python -m pip install -r requirements.txt``

Download This Project Zip Folder and Extract it

Move to project folder in Terminal. 
Then run following Commands :

``py manage.py makemigrations``

``py manage.py migrate``

``py manage.py runserver``

Now enter following URL in Your Browser Installed On Your Pc

``http://127.0.0.1:8000/``

# To containarize the app

`` docker-compose up --build``

you can see the two containers for both DB and web on docker desktop

# To Run app on AWS 

1.launch the EC2

2. VPC

3. Internet gatway

4. Security group

5. Subnets

6. MYSQL RDS

## on your EC2

install Docker

git clone the repo 

change settings.py file with the DB in RDS

to run the app in the background in order to makemigrations 

``docker-copmose up -d``


now you can write in terminal ``docker-compose exec web /bin/bash``

``python manage.py makemigrations``

``python manage.py migrate``

![image](https://github.com/user-attachments/assets/6a1ca502-25c8-44db-8e74-dab8a2823dfc)


![image](https://github.com/user-attachments/assets/94ff3b74-85d9-4f54-8745-bb9d3ca49204)


![image](https://github.com/user-attachments/assets/ca6763fb-0ecf-4874-a7a7-9c6f972882b7)
