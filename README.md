# AirBnB Clone - The Console

The console is the initial part of the AirBnB project at Holberton School, focusing on higher-level programming. The project's goal is to eventually deploy a simplified AirBnB website (HBnB). This console acts as a command interpreter to manage objects for the HBnB site.

#### Command Interpreter Features:
- Create new objects (e.g., User, Place)
- Retrieve objects from storage
- Perform operations on objects (e.g., count, compute stats)
- Update object attributes
- Destroy objects

## Table of Contents
- [Environment](#environment)
- [Installation](#installation)
- [File Descriptions](#file-descriptions)
- [Usage](#usage)
- [Examples of Use](#examples-of-use)
- [Bugs](#bugs)
- [Authors](#authors)
- [License](#license)

## Environment
Tested on Ubuntu 14.04 LTS using Python 3.4.3.

## Installation
- Clone this repository: `git clone "https://github.com/alexaorrico/AirBnB_clone.git"`
- Navigate to the directory: `cd AirBnB_clone`
- Run interactively: `./console`
- Run non-interactively: `echo "<command>" | ./console.py`

## File Descriptions
- **[console.py](console.py)**: Entry point for the command interpreter.
  - Commands: `EOF`, `quit`, `<emptyline>`, `create`, `destroy`, `show`, `all`, `update`

- **[models/](models/)**: Contains classes for this project.
  - [base_model.py](models/base_model.py): BaseModel class (foundation for other classes)
  - Derived classes: [amenity.py](models/amenity.py), [city.py](models/city.py), [place.py](models/place.py), [review.py](models/review.py), [state.py](models/state.py), [user.py](models/user.py)

- **[models/engine](models/engine/)**: Handles JSON serialization and deserialization.
  - [file_storage.py](models/engine/file_storage.py): Manages storage and retrieval of objects.

- **[tests/](tests/)**: Contains unit tests for the project.
  - Example: [test_base_model.py](tests/test_models/test_base_model.py)

## Examples of Use
```bash
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb) create BaseModel
7da56403-cc45-4f1c-ad32-bfafeb2bb050
(hbnb) all BaseModel
[[BaseModel] (7da56403-cc45-4f1c-ad32-bfafeb2bb050) {...}]
(hbnb) quit
```

## Bugs
No known bugs.

Author
- Dagmawi Yohannes

License