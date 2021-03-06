Process Management Project
=========================

Installation
-------------------------

#### NOTE: This README is copied from a different project directory. The use of MongoDB and React is TBD -- however, the instructions for setting up the Flask server remain the same ####

### Setting up MongoDB ###
Follow these installation instructions for [Mac](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/), [Windows](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/), and [Linux](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/) to setup `mongo` as a daemon on your machine.

### Clone repository ###

##### HTTPS #####
`git clone https://github.com/Aweeeezy/Process-Management-Project.git`

##### SSH #####
`git clone git@github.com:Aweeeezy/Process-Management-Project.git`

### Build back end ###

#### Create Python virtual environment ####
If you haven't already, install [Python 3.6](https://www.python.org/downloads/).

`cd Process-Management-Project/project/server/`

`python3.6 -m venv env`

`source env/bin/activate`

### Config database ###

#### Install MySQL Workbench ####
Install [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

Making alias

`alias mysql=/usr/local/mysql/bin/mysql`

`alias mysqladmin=/usr/local/mysql/bin/mysqladmin`


#### Install SQLAlchemy ####
Install [SQLAlchemy](http://docs.sqlalchemy.org/en/latest/intro.html).

`pip install SQLAlchemy`

In case you have not install pip

`sudo easy_install pip`


#### Install Python dependencies and set environment variables ####
`python3.6 -m pip install -e .`

`export FLASK_APP=pmgmt`

`export FLASK_DEBUG=true`

#### Run Flask server ####
`flask run`

### Build front end ###

#### Setting up React ####

If you haven't already, install [Yarn](https://yarnpkg.com/lang/en/docs/install/).

`cd Process-Management-Project/project/client/<deployment_option:={iOS, Android, Web}>/`

`yarn install`

#### Run React server ####
`yarn start`
