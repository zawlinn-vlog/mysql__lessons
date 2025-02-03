[![RDBMS](https://img.shields.io/badge/mySQL_lessons-000?style=for-the-badge&logo=ko-fi&logoColor=white)](#)

> I'm Zaw Linn Tun a Frontend Web Developer on [Zaw Linn - Vlog](https://www.youtube.com/@zawlinn-vlog). :heart:

<!-- #### PROJECT SIMPLE &mdash; -->

<!-- ![PROJECT_IMG](./assets/img/sample.png) -->

<br>

## What is RDBMS &mdash;

- RDMS is Relational Database Management System
- Open Source and Free
- Ideal for both small and large applications
- very fast, reliable, scalable and easy to use
- cross platform
- compliant with the ANSI SQL standard
- first relased in 1995
- developed, destriuted and supported by Oracle Coporation
- RDBMS use sql queries to access the data in the database

<br/>

### HOW TO CREATE DATABASEs &mdash;

```sh
    CREATE DATABASE databasename;
```

or

```sh
    CREATE DATABASE IF NOT EXISTS databasename;
```

or with encoding system &mdash;

```sh
    CREATE DATABASE databasename CHARACTER SET utf8 COLLATE utf8_unicode_ci;
```

or

```sh
    CREATE DATABASE IF NOT EXISTS databasename CHARACTER SET utf8 COLLATE utf8_unicode_ci;
```

#### CHECK DATABASEs &mdash;

```sh
    SHOW DATABASES;
```

#### DELETE DATABASEs &mdash;

```sh
    DROP DATABASE databasename;
```

<br/>

### HOW TO CREATE TABLEs &mdash;

```sh
    CREATE TABLE tablename (
        column_name datatype,
        column_name datatype,
        column_name datatype,
        ...
        );
```

#### CHECK TABLEs &mdash;

```sh
    SHOW TABLES;
```

#### to check table of other database &mdash;

```sh
    SHOW TABLES FROM databasename;
```

or

```sh
    SHOW TABLES IN databasename;
```

#### to check tables name and table type &mdash;

```sh
    SHOW FULL TABLES;
```

#### to check tables name and table type of other database &mdash;

```sh
    SHOW FULL TABLES FROM databasename;
```

or

```sh
    SHOW FULL TABLES IN databasename;
```

#### to check structured of table &mdash;

```sh
    DESCRIBE tablename;
```

or

```sh
    DESC tablename;
```

or

```sh
    SHOW COLUMNS FROM tablename;
```

#### to check table of other database &mdash;

```sh
    SHOW COLUMNS FROM database.tablename;
```

or

```sh
    SHOW COLUMNS FROM tablename IN databasename;
```

#### RENAME TABLE &mdash;

```sh
    ALTER TABLE old_tablename RENAME TO new_tablename;
```

#### ADD NEW COLUMN to TABLES &mdash;

```sh
    ALTER TABLE tablename ADD new_column_name datatype;
```

or

```sh
    ALTER TABLE tablename ADD COLUMN column_name datatype FIRST/AFTER existing_column_name;
```

or

```sh
    ALTER TABLE tablename
    ADD COLUMN column_name datatype,
    ADD COLUMN column_name datatype,
    ....;
```

<br/>

> FIRST - First Field.

> After - AFTER an ITEM.

#### Modified COLUMN &mdash;

```sh
    ALTER TABLE tablename
    MODIFY column_name datatype;
```

or

```sh
    ALTER TABLE tablename
    MODIFY column_name datatype,
    MODIFY column_name datatype,
    MODIFY column_name datatype
    etc... ;
```

#### MOVE COLUME INSIDE DATABASE &mdash;

```sh
    ALTER TABLE tablename MODIFY column_name datatype AFTER column_name;
```

#### RENAME COLUMN &mdash;

```sh
    ALTER TABLE table CHANGE COLUMN old_column_name new_column_name datatype;
```

#### DELETE COLUMN &mdash;

```sh
    ALTER TABLE tablename DROP COLUMN col_name;
```

or

```sh
    ALTER TABLE tablename
    DROP COLUMN col_name,
    DROP COLUMN col_name,
    etc...;
```

#### DELETE TABLE &mdash;

```sh
    DROP TABLE tablename;
```

#### DELETE TABLE FROM OTHER DATABASE &mdash;

```sh
    DROP TABLE databasename.tablename;
```

or

```sh
    DROP TABLE IF EXISTS databasename.tablename;
```

##### DELETE MULTI TABLE &mdash;

```sh
    DROP TABLE databasename.tablename, databasename.tablename, databasename.tablename,...;
```

or

```sh
    DROP TABLE IF EXISTS databasename.tablename, databasename.tablename, databasename.tablename, ...;
```

### TURNCATE TABLE &mdash;

```sh
    TRUNCATE TABLE tablename;
```

or

```sh
    TRUNCATE TABLE databasename.tablename;
```

or

```sh
    DELETE FROM tablename;
```

```sh
    DELETE FROM databasename.tablename;
```

### NOT NULL

### AUTO INCREMNET &mdash;

> `primary key` must be integer and to connect between tables and shld be auto increment;

```sh
    CREATE TABLE tablename (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,username VARCHAR(255) NOT NULL UNIQUE);
```

or

```sh
    CREATE TABLE tablename (id INT NOT NULL AUTO_INCREMENT,username VARCHAR(255) NOT NULL UNIQUE, ADD PRIMARY KEY(id));
```

or

```sh
    ALTER TALBLE tablename ADD COLUMN id INT NOT NULL AUTO_INCREMENT, ADD PRIMARY KEY(id);
```

or

```sh
    ALTER TABLE tablename ADD COLUMN id INT NOT NULL PRIMARY KEY AUTO_INCREMENT;
```

REMOVE PRIMARY KEY

- to remove primary key we shld remove auto increment

```sh
    ALTER TABLE tablename column_name datatype;  # (without auto_increment)

    ALTER TABLE tablname column_name DROP PRIMARY KEY;
```

UNIQUE KEY &mdash;

```sh
    ALTER TABLE tablenmae ADD UNIQUE(indexname);
```

or

```sh
    ALTER TABLE tablename ADD CONSTRAINT index_name UNIQUE(columnname, columnname, etc.)
```

REMOVE UNIQUE &mdash;

```sh
    SHOW INDEX FROM tablename;
    ALTER TABLE tablename DROP INDEX indexname;
```

CLONE TABLE WITH DATA &mdash;

```sh
    CREATE TABLE IF NOT EXISTS newTablename AS SELECT * FROM oldTablename; # NO PRIMARY, UNIQUE, AUTO_INCREMENT
```

<br/>

<!-- ![Screenshot of Project](./s1.png) -->

What I use packages are &mdash;

[![My Skills](https://skillicons.dev/icons?i=mysql,npm,git,github,vscode&perline=3)](https://skillicons.dev)

<br>

[![mySQL: Introduction](https://img.shields.io/badge/Relational_Database_Management_System_—-000?style=for-the-badge—=ko-fi—=white)](#)

📫 Reach me out!

[![Facebook Badge](https://img.shields.io/badge/-@zawlinn_vlog-1ca0f1?style=flat&labelColor=1ca0f1&logo=facebook&logoColor=white&link=https://faebook.com/zawlinn_profile)](https://facebook.com/zawlinn.vlog)
[![youtube Badge](https://img.shields.io/badge/-zawlinn_vlog-c0392b?style=flat&labelColor=c0392b&logo=youtube&logoColor=white)](https://youtube.com/@zawlinn-vlog)
[![Gamil Badge](https://img.shields.io/badge/-zawlinn.profile-c0392b?style=flat&labelColor=c0392b&logo=gmail&logoColor=white)](mailto:zawlinn.profile@gmail.com)

<!-- TODO: Add last video link -->

<details>
    <summary>
        My Portfolio
    </summary>
    <br/>

- :earth_asia: I’m currently working at @Mae Sot Market as a sale staff
- :computer: Most used line of code git commit -m "Initial Commit"
- :brain: I’m looking for help with Outstanding Video ideas.
- :mailbox_with_mail: How to reach me: zawlinn.profile@gmail.com.
- :heart: In a relationship with React
</details>
