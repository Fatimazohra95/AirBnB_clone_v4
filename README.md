AirBnB Clone - The Console
The console is a fundamental component of the AirBnB project at Holberton School, designed to manage objects for the AirBnB (HBnB) website. It serves as the first segment of the project, covering essential concepts of higher-level programming.

Functionalities
The goal of the AirBnB project is to deploy a server that mimics a simplified version of the AirBnB website. The command interpreter, implemented in this segment, provides the following functionalities:

Create a new object (e.g., a new User or a new Place)
Retrieve an object from a file, a database, etc.
Perform operations on objects (count, compute stats, etc.)
Update attributes of an object
Destroy an object
Table of Contents
Environment
Installation
File Descriptions
Usage
Examples of Use
Bugs
Authors
License
Environment
This project is interpreted and tested on Ubuntu 14.04 LTS using Python 3 (version 3.4.3).

Installation




git clone https://github.com/Fatimazohra95/AirBnB_clone.git



cd AirBnB_clone

./console


File Descriptions
console.py: The console contains the entry point of the command interpreter. It supports commands such as EOF, quit, create, destroy, show, all, and update.

models/: Directory containing classes used for this project.

base_model.py: The BaseModel class from which future classes will be derived.
__init__(self, *args, **kwargs): Initialization of the base model.
__str__(self): String representation of the BaseModel class.
save(self): Updates the attribute updated_at with the current datetime.
to_dict(self): Returns a dictionary containing all keys/values of the instance.
Usage

./console


Examples of Use

(hbnb) help
# Documented commands (type help <topic>):
# ========================================
# EOF  all  create  destroy  help  quit  show  update

(hbnb) all MyModel
# ** class doesn't exist **

(hbnb) create BaseModel
# 7da56403-cc45-4f1c-ad32-bfafeb2bb050

(hbnb) all BaseModel
# [[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}]

(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
# [BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}

(hbnb) destroy BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
# ** no instance found **

(hbnb) quit
Bugs
No known bugs at this time.

Authors
Fatima Zohra Lakhal - Github: https://github.com/Fatimazohra95


License
Public Domain. No copy write protection.
