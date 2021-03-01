# Software and Libraries Uses

- Oracle Autonomous Data Warehouse
- Python 3.8.5 requests bs4 shutil os zipfile cx_Oracle configparser pandas
- Tableau

# Setup

Once the database is running, run the create.sql statements to setup the tables and its relationships.

Create a folder called auth in the root directory. 
Extract the contents of the wallet file into this folder. 
Create a config.ini file and populate it with the below 3 lines.
```
[oracle]
username = username
password = password
```

The library cx_Oracle requires some .dll files. Download [Oracle Instant Client](https://www.oracle.com/database/technologies/instant-client/winx64-64-downloads.html) and extract the .dll files into your Python or virtual environment.

Update the Easy Connect String in etl.py with the appropriate TNS name. 
