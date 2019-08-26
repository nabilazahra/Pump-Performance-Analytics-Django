# Pump-Performance-Analytics-Django

A pump performance analytics data daashboard web app built with Django and JavaScript library Chart.js as the key graphic element. Data is received through CloudMQTT as the MQTT broker, with the publisher script running on the IOT Gateway. Warnings of the system are also sent through a Telegram chatbot.

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
```
Python 3.7.4
```
Python to be up and running on your terminal, and can perform pip. Installing on a virtual environment is advised.

### Installing
Run terminal on the project folder
```
$ pip install -r requirements.txt
```
### Authentication
Before deploying the server, fill in the authentication of the CloudMQTT broker and the telegram server in both the views.py and pub.py scripts.

### Deploying
To run the server,
```
$ python manage.py runserver
```
and the web app is deployed in http://127.0.0.1:8000/

(make sure you have the pub.py script running on the IOT Gateway first)

## Built With
* [Django](https://www.djangoproject.com) - The web framework used
* [chart.js](https://www.chartjs.org) - JavaScript library for the charts
* [REST Framework API](https://www.djangoproject.com) - Web API Builder Used
