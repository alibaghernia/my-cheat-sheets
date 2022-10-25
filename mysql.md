# create database
```sql
CREATE DATABASE db_name CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```
# import db
```bash
mysql -u root -p db_name < file_path.sql
```
# remove db
```sql
DROP DATABASE db_name;
```
# dump db
```bash
mysqldump -p -u root db_name > db_path.sql
```
```bash
mysqldump --no-data --skip-comments --skip-extended-insert -u root -p db_name>file2.sql
```
```bash
mysqldump --skip-comments --skip-extended-insert -u root -p db_name > db_path.sql
```
# show all databases
```sql
SHOW DATABASES;
```
