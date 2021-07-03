# Simple Firestore Import

Easily import data into Firebase Cloud Firestore from json and yaml files.

## Installation

Clone the repo:

    $ git clone 

Move into the directory:

    $ cd import_data_simple
    
Install dependencies:

    $ pip install -r requirements.txt

## Usage

Provide your **Firebase or Google Cloud service account key**, data file and the name of the collection.

    $ python import_data_firestore.py [path/to/service_account.json] [path/to/dataFile(.json|.yaml|.yml)] [name of collection]
    
Or without arguments:

    $ python import_data_firestore.py
    Path to serviceAccountKey.json: [path/to/service_account.json]
    Path to data file: [path/to/dataFile(.json|.yaml|.yml)]
    Name of collection: [name of collection]

Ex: 
    $ python import_data_firestore.py service_account.json data.json user
    
#### Note

The program expects an array of objects (dictionaries) to work.

**CORRECT DATA FILE FORMAT**

```json
[
    {
        "name": "Vien Nguyen",
        "email": "thevien898@gmail.com"
    },
    {
        "name": "Fiction",
        "email": "thevien@gmail.com"
    }
]
```

```yaml

---
- name: Vien Nguyen
  email: thevien898@gmail.com
- name: Fiction
  email: thevien@gmail.com
```