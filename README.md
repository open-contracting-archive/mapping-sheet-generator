*This is an OCDS Labs script: no guarantees as to the stability or operation of the script are provided*

# JSON Schema Mapping Spreadsheet Generator

This script will generate a spreadsheet that includes all possible field paths represented in an OCDS schema. 

To do this it will:

* Resolve all references in the schema;
* Make sure descriptions from the parent object containing a reference are maintained;
* Check for deprecation information

This version of the script can be run with the URL to a schema provided as the first parameter, or without, in which case it will look for a file named release-schema.json in the same folder.

The output is written to fields.csv


## Installation

```
virtualenv .ve --python=/usr/local/bin/python3.4
source .ve/bin/activate
pip install -r requirements.txt
```

