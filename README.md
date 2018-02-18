# django-react-starter
django 2.0 and reactjs starter template

This is based enitrely on: http://v1k45.com/blog/modern-django-part-1-setting-up-django-and-react/ 

The frontend config is identical to the github repo based on this article, but the django layout is different based on my preferences. It has a main app with a templates folder and some syntax changes updated for django2.0. The idea here is to try to provide a template that will allow you to potentially use react only in the parts of the app you want, as a opposed to a strict SPA/REST API style app. 

For a new dev setup:
Install a py3 venv and load the template as a new project...

```
django-admin startproject testapp --template=https://github.com/bsnacks000/django-react-starter/archive/master.zip --extension=json,js
```
activate venv and install for django 2 and webpack loader plugin
```
pip install -r requirements.txt
```
install the frontend and run the webpack server for development (port 3000)
```
cd frontend
npm install
npm start 
```
Boot the django server on 8000. You should see the sample ReactJS start app. You can now modify the React code dynamically.
