# ItemCatalog

Description

The code is written in Python 2.7. The program creates a web interface to interact with a recipe sql database.  Access to some pages are restricted to users logged in via Google.  Home page will show all the recipe types and the 10 most recent recipes added.  

Requirements 

sqllite3
sqlalchemy
Python 2.7
Vagrant VirtualBox

Setup

Database Set-Up 
Install VirtualBox Install Vagrant Use the following configuration file https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f73b_vagrantfile/vagrantfile newsdata.sql database is required. https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip

Execute

Running command With the database properly setup Start vagrant using vagrant up Log into vagrant using vagrant ssh change directory into folder containing recipe.py.  Type python recipe.py to run.   With the server now running you can open a browser and navigate to localhost:// to view the home page.  All database modifications require login with a google id.  

# JSON APIs to view recipes
All Recipes
/recipes/JSON

Individual User Recipes
/recipes/<int:user_id>/JSON

Recipes by type
/recipes/<string:type>/JSON
