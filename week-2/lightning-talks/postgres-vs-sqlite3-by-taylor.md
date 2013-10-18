## Postgress vs SQLite3

* Install postgres (see topher!)
* Modify your environment to access the postgres database from your app
``` 
DATABASE_URL = "postgres://localhost/mydb"
```
* Create the database `createdb mydb`

* Remove the database `dropdb mydb`

* Add to a rake file.
```
%x(createdb mydb)  
%x(dropdb mydb)
```

* Run `psql mydb` to see your database. 

* In `psql` you can see your schema by running commands:
  * `\dt` list all tables.
  * `\d table_name` to see schema of the table. 

