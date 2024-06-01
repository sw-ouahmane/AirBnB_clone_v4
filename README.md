# AirBnB Clone v4

<img src="https://s3.amazonaws.com/intranet-projects-files/concepts/74/hbnb_step5.png" width="600px">

### Description
Project attempts to clone the the AirBnB application and website, including the database, storage, RESTful API, Web Framework, and Front End.

### Concepts learned for phase 4:
* How to modify an HTML element style
* How to get and update an HTML element content
* How to modify the DOM
* How to make a GET request with jQuery Ajax
* How to make a POST request with jQuery Ajax
* How to listen/bind to DOM events
* How to listen/bind to user events

### Environment
Our AirBnB clone has been tested on Ubuntu 14.05.5 LTS
Tests done in VirtualBox on [Ubuntu](https://atlas.hashicorp.com/ubuntu/boxes/trusty64) via [Vagrant](https://www.vagrantup.com/)(1.9.1)

### The console functionality
* create your data model
* manage (create, update, destroy, etc) objects via a console / command interpreter
* store and persist objects to a file (JSON file)

## Console Execution
First step is to clone the repository into your directory:
``` 
$ git clone https://github.com/halinav00/AirBnB_clone.git 
```
To run the console, type `./console.py` script. 
```
$ ./console.py
```
Type `help` for list of commands.
```
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb)
```

Commands include:
* `create`: creates a new instance of model (you need to specify class for the model)
* `show`: shows information about a model based on id
* `destroy`: delete model
* `all`: display information about all models
* `update`: updates instance based on name, id and attribute
* `quit`: exits


## API execution:
on port 5000:
```
guillaume@ubuntu:~/AirBnB_v4$ HBNB_MYSQL_USER=hbnb_dev HBNB_MYSQL_PWD=hbnb_dev_pwd HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_dev_db HBNB_TYPE_STORAGE=db python3 -m web_dynamic.0-hbnb
* Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
```
API execution on port 5001:
```
guillaume@ubuntu:~/AirBnB_v4$ HBNB_MYSQL_USER=hbnb_dev HBNB_MYSQL_PWD=hbnb_dev_pwd HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_dev_db HBNB_TYPE_STORAGE=db HBNB_API_PORT=5001 python3 -m api.v1.app
...
```

**Examples of front end:**:

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/309/hbnb_2_0.jpg)

![](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/309/hbnb_1_2.jpg)

**Examples of console use:**
```
(hbnb) create User
3db5637d-5df4-44cf-a250-ef2b523946e9
(hbnb) show User 3db5637d-5df4-44cf-a250-ef2b523946e9
[User] (3db5637d-5df4-44cf-a250-ef2b523946e9) {'id': '3db5637d-5df4-44cf-a250-ef2b523946e9', 
       'updated_at': datetime.datetime(2017, 6, 13, 4, 18, 50, 138053), 'created_at': 
       datetime.datetime(2017, 6, 13, 4, 18, 50, 138027)}
(hbnb) destroy User 3db5637d-5df4-44cf-a250-ef2b523946e9
(hbnb) show User 3db5637d-5df4-44cf-a250-ef2b523946e9
** no instance found **
(hbnb)
```



## Author


* Abdallah OUAHMANE, [@ouahmane](https://github.com/sw-ouahmane)
