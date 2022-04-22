# HARD: Hedging Agricultural Risk Dashboard

Open-source **[Dashboard](https://cse6242team45.github.io/)**. It provides an interactive dashboard for farmers and ranchers to gather comprehensive information on agricultural information, including geographic data visualization on yields, production, and sales for a vareity of crops (e.g., wheat, corns, barley, soybeans, and potatoes). Using the data from the **[United States Department of Agriculture (USDA)](https://www.usda.gov/)**, the dashboard also provides price predictions generated by the trained time series models to guide risk management and decision making for farmers and ranchers.

<br />

> Features

- Visualization of `crop production` on the geomap
- Visualization of `crop yields` on the geomap
- Visualization of `crop sales` on the geomap
- `Crop price prediction` from time series models
- `Data download` functionality

<br />

> Links

- 👉 [Background](https://cse6242team45.github.io/)
- 👉 [Video Demo](https://cse6242team45.github.io/)

<br />

## ✨ Implementation and Development

> Get the code

```bash
$ git clone https://github.com/CSE6242Team45/CSE6242Team45.github.io.git
$ cd CSE6242Team45.github.io.git
```
Make the desired modifications and host the code in your own git repo (see more instructions in the **Project Host** section below).

<br />

![Screen Capture.](/screencaptures/dashboard1.png)

<br />

## ✨ Project Host

The app is hosted by **[GitHub Pages](https://pages.github.com/)**.

<br />

> General steps to host any project on **GitHub Pages**:

- [Create a repo](https://github.com/new) on GitHub
- Clone the repository
- Add, commit, and push your files (e.g., HTML)
- Open a browser and go to https://username.github.io

<br />

## ✨ Code-base structure

The project is coded using blueprints, app factory pattern, dual configuration profile (development and production), and an intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- apps/
   |    |
   |    |-- home/                           # A simple app that serve HTML files
   |    |    |-- routes.py                  # Define app routes
   |    |
   |    |-- authentication/                 # Handles auth routes (login and register)
   |    |    |-- routes.py                  # Define authentication routes  
   |    |    |-- models.py                  # Defines models  
   |    |    |-- forms.py                   # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>          # CSS files, Javascripts files
   |    |
   |    |-- templates/                      # Templates used to render pages
   |    |    |-- includes/                  # HTML chunks and components
   |    |    |    |-- navigation.html       # Top menu component
   |    |    |    |-- sidebar.html          # Sidebar component
   |    |    |    |-- footer.html           # App Footer
   |    |    |    |-- scripts.html          # Scripts common to all pages
   |    |    |
   |    |    |-- layouts/                   # Master pages
   |    |    |    |-- base-fullscreen.html  # Used by Authentication pages
   |    |    |    |-- base.html             # Used by common pages
   |    |    |
   |    |    |-- accounts/                  # Authentication pages
   |    |    |    |-- login.html            # Login page
   |    |    |    |-- register.html         # Register page
   |    |    |
   |    |    |-- home/                      # UI Kit Pages
   |    |         |-- index.html            # Index page
   |    |         |-- 404-page.html         # 404 page
   |    |         |-- *.html                # All other pages
   |    |    
   |  config.py                             # Set up the app
   |    __init__.py                         # Initialize the app
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |-- requirements-mysql.txt               # Production modules  - Mysql DMBS
   |-- requirements-pqsql.txt               # Production modules  - PostgreSql DMBS
   |
   |-- Dockerfile                           # Deployment
   |-- docker-compose.yml                   # Deployment
   |-- gunicorn-cfg.py                      # Deployment   
   |-- nginx                                # Deployment
   |    |-- appseed-app.conf                # Deployment 
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- run.py                               # Start the app - WSGI gateway
   |
   |-- ************************************************************************
```
<br />

## ✨ Credits & Links

- [Dashboard Framework](https://cse6242team45.github.io/)
- [USDA Data Source](https://quickstats.nass.usda.gov/)
- [Course Link](https://omscs.gatech.edu/cse-6242-data-visual-analytics)

<br />