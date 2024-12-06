# Ex.06 Book Front Cover Page Design
# Date:
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
### views.py
```
from django.shortcuts import render

def book(request):
    return render(request,'web.html')
```
### settings.py
```


from pathlib import Path
import os


BASE_DIR = Path(__file__).resolve().parent.parent



SECRET_KEY = 'django-insecure-pg%ap8h4b8g+^gyw$cwuxx_nyzc(y&_&ngc0qi4nfxha4i_a%x'


DEBUG = True

ALLOWED_HOSTS = []


INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'app',
]

MIDDLEWARE = [
    'django.middleware.security.SecurityMiddleware',
    'django.contrib.sessions.middleware.SessionMiddleware',
    'django.middleware.common.CommonMiddleware',
    'django.middleware.csrf.CsrfViewMiddleware',
    'django.contrib.auth.middleware.AuthenticationMiddleware',
    'django.contrib.messages.middleware.MessageMiddleware',
    'django.middleware.clickjacking.XFrameOptionsMiddleware',
]

ROOT_URLCONF = 'manikandan.urls'

TEMPLATES = [
    {
        'BACKEND': 'django.template.backends.django.DjangoTemplates',
        'DIRS': [],
        'APP_DIRS': True,
        'OPTIONS': {
            'context_processors': [
                'django.template.context_processors.debug',
                'django.template.context_processors.request',
                'django.contrib.auth.context_processors.auth',
                'django.contrib.messages.context_processors.messages',
            ],
        },
    },
]

WSGI_APPLICATION = 'manikandan.wsgi.application'



DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}



AUTH_PASSWORD_VALIDATORS = [
    {
        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
    },
    {
        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
    },
]


m/en/5.1/topics/i18n/

LANGUAGE_CODE = 'en-us'

TIME_ZONE = 'UTC'

USE_I18N = True

USE_TZ = True



STATIC_URL = 'static/'


DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'

```
### urls.py
```from django.contrib import admin
from django.urls import path
from app import views
urlpatterns = [
    path('admin/', admin.site.urls),
    path('book',views.book)
]
```
### web.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>* {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    
    body {
        font-family: sans-serif;
        line-height: 1;
        color: white;
    }
    
    a {
        text-decoration: none;
    }
    
    li {
        list-style: none;
    }
    
    
    .expert-insight {
        margin: 10px 50px;
    }
    
    
    .custom-hr {
        width: 30%;
        margin: 0;
        border: none;
        border-top: 3px solid rgb(44, 41, 40);
        margin-left: 0;
    }
    
    .heading {
        margin: 10px 50px;
        font-size: 4rem;
    }
    
    .sub-heading {
        margin: 10px 50px;
        font-size: 1.4rem;
        font-weight: 550;
        line-height: 1;
    }
    
    
    .spiral-image {
        width: 600px;
        padding: 0px;
        margin: 0px;
    }
    
    
    .editon-image-div {
        margin: 10px 50px;
        display: flex;
        justify-content: space-between;
        align-items: end;
    }
    
    .third-edition {
        font-size: x-large;
        font-weight: 800;
        color: rgb(248, 70, 0);
    }
    
    .ben-image {
        width: 350px;
        
    }
    
    .custom-full-hr {
        border: 1px solid rgb(248, 70, 0);
    }
    
    .author-div {
        margin: 10px 50px;
    }
    
    .author-div { 
        display: flex;
        justify-content: space-between;
        padding: 20px 0;
    }
    
    .ben-frain {
        font-size: 1.6rem;
        font-weight: 600;
    }
    
    .packt {
        font-size: 2rem;
        font-weight: 515;
        text-decoration: underline;
    }
    .one{
        width: 600px;
        height: 800px;
        background-color: rgb(9, 9, 9);
    }
    </style>
</head>
{% load static %}

<body>
    <center>
    <div class="one">
    <p class="expert-insight">EXPERT INSIGHT</p>
    <hr class="custom-hr">
    <h1 class="heading">Responsive Web <br> Design with <br> HTML5 and CSS</h1>
    <p class="sub-heading">Develop future-proof responsive websites <br> using the latest HTML5 and CSS3 techniques</p>
    <div class="spiral-image-div">
        <img src="{% static 'images/sp3.png'%}"height="40%" width="35%">
    </div>
    <div class="editon-image-div">
        <p class="third-edition">Third Edition</p>
        <img src="{% static 'images/pic7.png'%}"height="45%" width="35%">
    </div>
    <hr class="custom-full-hr">
    <div class="author-div">
        <p class="ben-frain">MANIKANDAN V</p>
        <p class="packt">Packt</p>
    </div>
</div>
    </center>
</body>

</html>
```
# OUTPUT:

![Screenshot 2024-12-05 141003](https://github.com/user-attachments/assets/f8d5dcd8-7e07-4259-b8a2-816a5956fd99)

# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
