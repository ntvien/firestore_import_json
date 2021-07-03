## Installation

Clone the repo:

    $ git clone https://github.com/ntvien/firestore_import_json

Move into the directory:

    $ cd import_data_env
    
## SETTING UP YOUR VIRTUAL ENVIRONMENT

For Mac:

    $ pip install virtualenv
    $ virtualenv <your-env>
    $ pip install google-cloud-firestore

For Window:

    $ pip install virtualenv
    $ virtualenv <your-env>
    $ cd <your-env>/Scripts
    $ pip install google-cloud-firestore

## Usage

Method Set:

    $ python import_json_to_firestore.py data.json set country

Method Add:

    $ python import_json_to_firestore.py data.json add country