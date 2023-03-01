+++ 
draft = false
title = "Django data app - from prototype to 1.0 "
tags = ["django","python","heroku"]
categories = ["portfolio"]
+++
[Go to django app](http://djangoapp.falko.in)

## Goals

After successfully prototyping a data app with [Streamlit](https://streamlit.io/) to explore trampoline data the next step was to develop a more sophisticated variant with [Django](https://www.djangoproject.com/).  

Things that were on the to-do list:
- User-login
- Data-upload for admins
- Comparison of athletes

## Technical aspects

- Data upload as csv via [dropzone.js](https://www.dropzone.dev/) into data models
- Data processing with [pandas](https://pandas.pydata.org/)
- Visualization with [plotly](https://plotly.com/python/) 
- MySQL database at [Google Cloud Platform](https://cloud.google.com)
- Django app deployed with [Heroku](https://heroku.com)
- Frontend with HTML, CSS, Bootstrap, Javascript
