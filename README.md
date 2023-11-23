# AirBnB Clone - Console Overview

The console marks the initial phase of the AirBnB project at Holberton School, serving as the foundation for exploring essential concepts in higher-level programming. The ultimate objective of the AirBnB project is to deploy a server mirroring the AirBnB Website (HBnB). This segment introduces a command interpreter designed to manage objects for the AirBnB (HBnB) website.

Command Interpreter Functionalities:
Create a new object (e.g., User or Place)
Retrieve an object from a file, database, etc.
Perform operations on objects (count, compute stats, etc.)
Update attributes of an object
Destroy an object
Table of Contents:
Environment
Installation
File Descriptions
Usage
Examples of Use
Bugs
Authors
License
Environment:
This project is interpreted and tested on Ubuntu 14.04 LTS using Python 3 (version 3.4.3).

Installation:
Clone this repository: git clone "https://github.com/alexaorrico/AirBnB_clone.git"
Access AirBnb directory: cd AirBnB_clone
Run hbnb (interactively): ./console and enter commands
Run hbnb (non-interactively): echo "<command>" | ./console.py
File Descriptions:
console.py
The console contains the entry point of the command interpreter. It supports various commands, including create, destroy, show, all, and update.

models/ directory
Contains classes used for this project:

base_model.py: The BaseModel class from which future classes will be derived.
amenity.py, city.py, place.py, review.py, state.py, user.py: Classes inherited from BaseModel.
models/engine directory
Contains the FileStorage class responsible for JSON serialization and deserialization:

file_storage.py: Serializes instances to a JSON file and deserializes back to instances.
/tests directory
Includes all unit test cases for this project:

test_models/test_base_model.py, test_models/test_amenity.py, test_models/test_city.py, test_models/test_file_storage.py, test_models/test_place.py, test_models/test_review.py, test_models/test_state.py, test_models/test_user.py: Test classes for various modules.
Usage:
Execute ./console.py to enter the console.
Use commands like create, destroy, show, all, and update to manage objects.
Examples of Use:
bash
Copy code
vagrantAirBnB_clone$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb) all MyModel
** class doesn't exist **
(hbnb) create BaseModel
7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) all BaseModel
[[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}]
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {'updated_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772167), 'id': '7da56403-cc45-4f1c-ad32-bfafeb2bb050', 'created_at': datetime.datetime(2017, 9, 28, 9, 50, 46, 772123)}
(hbnb) destroy BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) show BaseModel 7da56403-cc45-4f1c-ad32-bfafeb2bb050
** no instance found **
(hbnb) quit
Feel free to explore and manipulate objects using the provided commands within the console environment.

## Bugs
No known bugs at this time. 

## Authors
Job Kimani - [Github](https://github.com/Jobkimani) /   
JUDE MAUNDU - 
## License
Public Domain. No copy write protection. 
