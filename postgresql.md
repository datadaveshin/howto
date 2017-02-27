# Load a .csv file
http://stackoverflow.com/questions/2987433/how-to-import-csv-file-data-into-a-postgresql-table
http://web.archive.org/web/20101030205652/http://ensode.net/postgresql_csv_import.html

###Make the table:
```
CREATE TABLE zip_codes 
(ZIP char(5), LATITUDE double precision, LONGITUDE double precision, 
CITY varchar, STATE char(2), COUNTY varchar, ZIP_CLASS varchar);
```

###Copy data from your CSV file to the table:
```
COPY zip_codes FROM '/path/to/csv/ZIP_CODES.txt' DELIMITER ',' CSV;
```

