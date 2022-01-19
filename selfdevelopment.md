Self Development project Notes

We use Django for API
React-Redux for front-end

Step: 1. Choosing a project
Step: 2. QuickStart App
Step: 3. Designing
Step: 4. Django API
Step: 5. Frontend
Step: 6. Testing and Debugging
Step: 7. Deployment of project

Useful Links:
(QuickStartApp Repository Link) https://github.com/Tech-i-s/techis-wd-forum-django-react.git
Backend
1. Understand the app requirements, create the Apps in the backend accordingly.
Create the apps in Apps Folder
python manage.py -m django startapp (appname)
2. In the config folder add the urls and in settings.py register the apps.

3. Create Serializers in all the apps folders and other requirements like forms urls etc.
Serializer
Serializers are for to pass information in bits and also when you want to store it in redux
Models.py
In models.py, we design app structure and models. Creating tables for the models
Views.py
In views.py, we design the function for each model and how they are displayed.
Constants.py
Constants are like the constant words across the project.

Frontend
1. In frontend we'll first design the HTML CSS files for the App.

2. Will convert the HTML's into.JSX format.
Folder Structure
Assets: In assets, we'll add all the common images like logos, Background images etc those are fixed for the entire page.
Components: In the components folder, we'll divide the page into sections and add all the common sections in a subfolder called components.
Container: In the container folder, we'll create all the main pages like the Home page, Cart page etc.
Redux: In the redux folder, we'll create the 
* Action
* Operation
* Reducer
* Selector
and also Store

Action: We'll create all the activities that are carried out on the particular page
Operation: We'll define the operations on how the actions take place
Reducer: Defines the state after performing each operation
Selector: Selects the particular items required for performing the actions.

API.js
In API.js, we'll be linking the Django API and writing the functionalities for operations to be carried out for the entire WebApp with the help of API.

APP.js
In App.js, we'll define the structure of the app. How the sections should display in the app.

Router.jsx
In the router, we'll add the path for all the pages created in the container folder.
Index.js
Index.js is that of an index page in a book that contains all the contents across it.

USEFUL Codes for Django

Django Codes Windows

Creating Environment
Python -m env env

Activating Environment
Env\Scripts\activate

Creating Django Project
Python -m Django startproject projectname

Creating Django Application like posts carts users
Python -m django start app app name

Makemigrations
Python manage.py makemigrations

Migrating		( always try to migrate when you make changes to views.py models.py )
Python manage.py migrate

Running the server
Python manage.py runserver

If any errors like module not found
Pip install that module name

pip freeze > requirements.txt 
pip install django-heroku
python manage.py createsuperuser

pip install cloudinary
pip install django-cors-headers
pip install djangorestframework
pip install django-filter
pip install Pillow
pip install 
source venv/bin/deactivate
pip install psycopg2-binary

Heroku Deployment

1. Create a pipeline
2. Create production app for backend and Frontend
3. Connect with GitHub Repository
4. Enable automatic deploys
Frontend
1. In Settings 
   var config: add PROJECT_PATH as FRONTEND
2. Add build packs
https://github.com/timanovsky/subdir-heroku-buildpack
https://github.com/mars/create-react-app-buildpack
3. Make sure about the order of build pack is same as mentioned
4. Deploy
Backend
1. In Resources add Heroku Postgress
2. Add the credentials in settings.py
3. In settings of Heroku add the PROJECT_PATH as backend in var config
4. Add the build pack
https://github.com/timanovsky/subdir-heroku-buildpack
heroku/python
5. Make sure you have clicked on python Logo after typing heroku/python
6. Deploy

If an application error occurs while deploying the backend, go to code and check the Database.
