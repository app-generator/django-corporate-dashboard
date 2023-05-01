# Django Corporate Dashboard

Open-source **Django** project crafted on top of **Corporate Dashboard**, an open-source `Bootstrap 5` design from [Creative-Tim](https://www.creative-tim.com/product/corporate-ui-dashboard?AFFILIATE=128200).
Designed for those who like bold elements and beautiful websites. Made of hundred of elements, designed blocks and fully coded pages, `Corporate Dashboard` is ready to help you create stunning websites and webapps.

- 👉 [Django Corporate Dashboard](#) - `Product page` (soon)
- 👉 [Django Corporate Dashboard](#) - `LIVE Demo` (soon)
- 🚀 Free [Support](https://appseed.us/support/) via Email & `Discord`

<br />

> Features: 

- ✅ `Up-to-date Dependencies`
- ✅ Theme: [Django Admin Corporate](https://github.com/app-generator/django-admin-corporate), designed by [Creative-Tim](https://www.creative-tim.com/product/corporate-ui-dashboard?AFFILIATE=128200)
  - `can be used in any Django project` (new or legacy)
- ✅ **Authentication**: `Django.contrib.AUTH`, Registration
- 🚀 `Deployment` 
  - `CI/CD` flow via `Render`
  - [Django Soft - Go LIVE](https://www.youtube.com/watch?v=1QVdQVSkUCI) - `video presentation`

<br />

![Django Corporate Dashboard](https://user-images.githubusercontent.com/51070104/229719846-cfe96c5c-89c2-4ea0-89a9-7be69ebbb228.png)

<br />

## Manual Build 

> 👉 Download the code  

```bash
$ git clone https://github.com/app-generator/django-soft-ui-dashboard.git
$ cd django-soft-ui-dashboard
```

<br />

> 👉 Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

<br />

> 👉 Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> 👉 Create the Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> 👉 Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## Codebase structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                            
   |    |-- settings.py   # Project Configuration  
   |    |-- urls.py       # Project Routing
   |
   |-- home/
   |    |-- views.py      # APP Views 
   |    |-- urls.py       # APP Routing
   |    |-- models.py     # APP Models 
   |    |-- tests.py      # Tests  
   |     
   |-- templates/
   |    |-- includes/     # UI components 
   |    |-- layouts/      # Masterpages
   |    |-- pages/        # Kit pages 
   |
   |-- static/   
   |    |-- css/                                   # CSS Files 
   |    |-- scss/                                  # SCSS Files 
   |         |-- corporate-ui-dashboard/_variables.scss # File Used for Theme Styling
   |
   |-- requirements.txt   # Project Dependencies
   |
   |-- env.sample         # ENV Configuration (default values)
   |-- manage.py          # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## Recompile SCSS  

The SCSS/CSS files used to style the Ui are saved in the `static` directory. 
In order to update the Ui colors (primary, secondary) this procedure needs to be followed. 

```bash
$ yarn                                                  # install modules
$ vi static/scss/corporate-ui-dashboard/_variables.scss # edit variables 
$ gulp                                                  # SCSS to CSS translation
```

The `_variables.scss` content defines the `primary` and `secondary` colors: 

```scss
$primary:       #774dd3 !default; // EDIT for customization
$secondary:     #64748b !default; // EDIT for customization
$info:          #55a6f8 !default; // EDIT for customization
$success:       #67c23a !default; // EDIT for customization
$warning:       #f19937 !default; // EDIT for customization 
$danger:        #ea4e3d !default; // EDIT for customization
```

<br />

## Deploy on [Render](https://render.com/)

- Create a Blueprint instance
  - Go to https://dashboard.render.com/blueprints this link.
- Click `New Blueprint Instance` button.
- Connect your `repo` which you want to deploy.
- Fill the `Service Group Name` and click on `Update Existing Resources` button.
- After that your deployment will start automatically.

At this point, the product should be LIVE.

<br />

---
[Django Soft Dashboard](https://appseed.us/product/soft-ui-dashboard/django/) - **Django** starter provided by **[AppSeed](https://appseed.us/)**
