# Flask-app with mysql

Info:

You can configure a Flask app an mysql database as containerize on K8S cluster using Vagrant.
I dockerized flesk app with alpine:3.7 base image. You can find dockerfile in PythonApp folder.
I also added two deployment yaml both mysql and flask application. I also added necessary service definition on these yaml files.
I genereted a secret for mysql requirements. This secret has been used on yaml files as secret key reference.
And I used weave network plugin for cni.
Last but not least I created persistent volume and persistent volume claim to make mysql data persistent.

Requirements:

1- Virtual Box 6.0

2- Vagrant


Quick Start:

1. Clone this repo.
2. Boot up your vagrant environment.

Nodes: 

![Nodes](https://github.com/yasarfirat/python-app/blob/master/Pics/Nodes.jpg)

Deployments:

![Deployments](https://github.com/yasarfirat/python-app/blob/master/Pics/deployments.jpg)

Application:

![Application](https://github.com/yasarfirat/python-app/blob/master/Pics/application.jpg)
