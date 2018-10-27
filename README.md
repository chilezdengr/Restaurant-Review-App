# Restaurant Review Application
---
## Table of Contents

* [Installation](#installation)
* [Navigating the Webpage](#navigating)
* [Restriction](#restriction)


Restaurant Review App
## Overview
This project takes a site with static design that also lacks accessibility and converts the design to be responsive on different sized displays and accessible for screen reader use. It adds a service worker to ensure seemless experience for users.

## Installation
Get this project to your local machine by running git clone https://github.com/chilezdengr/Restaurant-Review-App.git in the terminal.

To run the app you need a simple HTTP server to serve up the site files on your local computer. Python has some simple tools to do this, and you don't even need to know Python. For most people, it's already installed on your computer.

In a terminal, check the version of Python you have: python -V. If you have Python 2.x, cd into the project home directory and spin up the server with python -m SimpleHTTPServer 8000 (or some other port, if port 8000 is already in use.) For Python 3.x, you can use python -m http.server 8000. If you don't have Python installed, navigate to Python's website to download and install the software.

Navigate to the js directory, open the dbhelper.js file and change the port to your preferred port, with your server running, visit the site: http://localhost:8000. Don't forget to replace the port in the address with whatever port you have chosen.

You can now access the web app on your browser .


## Restrictions
This app uses service worker to cache the resources needed to render this site. I have not used any build tool to compile my js. So right now there is no way to automatically update the service worker when you make changes to your scripts. You have to manually update the myCache variable in serviceworker file(serviceworker.js), each time you make updates to your scripts. Feel free to use a build tool (gulp or grunt) when your make changes to the code base.
