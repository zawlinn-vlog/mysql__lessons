[![RDBMS](https://img.shields.io/badge/mySQL_Lessons_—-000?style=for-the-badge—=ko-fi—=white)](#)

> I'm Zaw Linn Tun a Frontend Web Developer on [Zaw Linn - Vlog](https://www.youtube.com/@zawlinn-vlog). :heart:

<!-- #### PROJECT SIMPLE &mdash; -->

<!-- ![PROJECT_IMG](./assets/img/sample.png) -->

<br>

## Variables &mdash;

1. System Variables

   (i) GLOBAL Variables

   (ii) SESSION Variables

2. User-Defined Variables

3. Parameters and Local Variables

### SYSTEM VARIABLEs &mdash;

```sh
    SHOW VARIABLES;
```

or

```sh
    SELECT @@varname; # @@warning_count;
    SELECT @@error_count;
```

<br/>

> @@ -> System Variables

> @ -> User Defined Variables

### USER DEFINED VARIABLEs &mdash;

```sh
    SELECT @uservar := 'str'; # SELECT @myVar := 'Hello Myanmar';
    SELECT @myVar;
```

or

```sh
    SET @varName = 'str'; # SET @varName = 'Data Land';
    SELECT @varName;
```

eg.

```sh
    SELECT @num1 := '10';
    SELECT @num2 := '20';

    SELECT @num1+@num2;
```

or

```sh
    SELECT @num1 := '10';
    SELECT @num2 := '20';
    SELECT @num3 := '30';
    SELECT @num4 := '40';

    SELECT @num1,@num2,@num3,@num4;
    SELECT @num3*@num4;
```

CLEAR CMD &mdash;

```sh
    system clear;
```

### DATA TYPEs &mdash;

#### STRING DATA TYPEs &mdash;

| DATATYPE                  | DESCRIPTION                                                                               |
| ------------------------- | ----------------------------------------------------------------------------------------- |
| CHAR(size)                | A fixed length String (can contain letters, numbers, special characters) 0 - 255          |
| VARCHAR(size)             | A variable length String (can contain letters, numbers, special characters) 0 - 65535     |
| TEXT                      | Hold a string with maximum size 68,xxx (6kb)                                              |
| TINYTEXT                  | Hold a string with maximun size 255 (255bytes)                                            |
| MEDIUMTEXT                | Hold a string with maximun size 16,xxx,xxx (16mb)                                         |
| LONGTEXT                  | Hold a string with maximun size 4,xxx,xxx,xxx (4Gb)                                       |
| BINARY(size)              | Equal to CHAR(size), but store binary bit strings 0 - 255                                 |
| VARBINARY(size)           | Equal to VARCHAR(size), but store binary bit strings 0 - 255                              |
| BLOB()                    | For BLOB(Binary Large Objects), maximun size 68,xxx (6kb)                                 |
| TINYBLOB()                | For BLOB(Binary Large Objects), maximun size 255 (255b)                                   |
| MEDIUMBLOB()              | For BLOB(Binary Large Objects), maximun size 16,xxx,xxx (16mb)                            |
| LONGBLOB()                | For BLOB(Binary Large Objects), maximun size 4,xxx,xxx,xxx (4Gb)                          |
| ENUM('val1', 'val2', ...) | A String Object that can be only one value and choose from a lists you already defined    |
| SET('val1', 'val2', ...)  | A String Object that can be one value or more but choose from a lists you already defined |

CHAR

- CHAR is faster for fixed length TEXT (eg. telephone numbers, zip code, YES/NO, Y/N, Male, Female M/F)

CHAR(4) Vs VARCHAR(4)

USER INPUT

| VALUE     | CHAR(4)                           | Storage | VARCHAR(4) | Storage |
| --------- | --------------------------------- | ------- | ---------- | ------- |
| ''        | \' &nbsp; &nbsp; &nbsp; &nbsp; \' | 4bytes  | ''         | 1bytes  |
| 'ab'      | ' ab &nbsp; &nbsp; \'             | 4bytes  | 'ab'       | 3bytes  |
| 'abcd'    | 'abc &nbsp; \'                    | 4bytes  | 'abc'      | 5bytes  |
| 'abcdefg' | 'abcd'                            | 4bytes  | 'abcd'     | 5bytes  |

```sh
    CREATE TABLE IF NOT EXISTS items (id INT NOT NULL AUTO_INCREMENT, name VARCHAR(20), purchasePrice INT(4) SIGNED, sellprice INT(4) UNSIGNED, status BOOL, PRIMARY KEY (id));
```

and then

```sh
    INSERT INTO items (name, purchasePrice, sellprice, status) VALUES ('water', 9000, 9500, 0), ('coffee', -100, 200, 1), ('cake', 800, 100,0), ('snack', -250.56, 350.77, 1), ('jam', -1000, 2000, 0);
```

#### Numberic DATA TYPEs &mdash;

| DATATYPE                  | DESCRIPTION                                                                                    |
| ------------------------- | ---------------------------------------------------------------------------------------------- |
| BIT(size)                 | A bit-value type, from 1 to 64 (default value is 1)                                            |
| BOOL(size)                | Zero is considered as `FALSE`, Non-zero are considered as `TRUE`                               |
| BOOLEAN                   | Zero is considered as `FALSE`, Non-zero are considered as `TRUE`                               |
| TINYINT(size)             | A very small interger, Signed -128 to 127 and Unsigned 0 to 255 (1byte)                        |
| SMALLINT(size)            | A small interger, Signed -32768 to 32767 and Unsigned 0 to 65535 (2bytes)                      |
| MEDIUMINT                 | A medium interger, Signed -8388608 to 8388607 and Unsigned 0 to 16777215 (3bytes)              |
| INT(size)                 | A interger, Signed -2147483648 to 2147483647 and Unsigned 0 to 4294967295 (4bytes)             |
| INTEGER                   | A interger, Signed -2147483648 to 2147483647 and Unsigned 0 to 4294967295 (4bytes)             |
| BIGINT()                  | A small interger, Signed -2147483648 to 2147483647 and Unsigned 0 to 4294967295 (8bytes)       |
| DECIMAL(size, d)          | Fixed-point number, default value for d is 0 eg.(999.99) is digit and 2 decimal - DECIMAL(5,2) |
| DEC(size, d)              | Fixed-point number, default value for d is 0                                                   |
| FLOAT(p) size is optional | A floating point number (Approximate Value), p is optional - p is from 0 to 24                 |
| DOUBLE(size, p)           | A floating point number (Approximate Value), p is optional - p is 25 to 53                     |

> NOTE: DECIMAL for Financial ( SUCH AS MONEY - POS)

> NOTE: FLOAT for SCIENCE APP

| TYPES   |                                                                                                                                                                  |                |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| integer | fixed-point                                                                                                                                                      | Floating-point |
| INTEGER | DECIMAL(Total Number of digits, Digit after decimal) eg. 999.99 is 5 digits and 2 decimal digits (fixed-point data type) eg. DECIMAL(5,3)= 20.234, 20.5 = 20.500 | FLOAT/DOUBLE   |

> NOTE: DECIMAL data type is fixed-point type and calculate are exact

> NOTE: FLOAT & DOUBLE data type are floating-point types and calculation are approximate.

```sh
    CREATE TABLE IF NOT EXIT purchases (id INT NOT NULL AUTO_INCREMENT, items VARCHAR(20) NOT NULL, price FLOAT, total FLOAT(4), PRIMARY KEY(id), UNIQUE(items));
```

<br />

#### DATE DATA TYPEs &mdash;

| DATATYPE  | DESCRIPTION                                                                                                                    |
| --------- | ------------------------------------------------------------------------------------------------------------------------------ |
| DATE      | A `DATE`, FORMAT: `YYYY-MM-DD`, The Support rang is from `1000-01-01` To `9999-12-31`.                                         |
| DATETIME  | A `DATE` and `TIME` combination, FORMAT `YYYY-MM-DD hh:mm:ss` the support range `1000-01-01 00:00:00` To `9999-12-31 23:59:59` |
| TIMESTAMP | A `TIMESTAMP` FORMAT `YYYY-MM-DD hh:mm:ss`                                                                                     |
| TIME      | A `TIME`. FORMAT `hh:mm:ss`                                                                                                    |
| YEAR      | A `YEAR` with four-digit fomat                                                                                                 |

<br/>

EXERCISE

```sh
    SELECT CURRENT_DATE(); ## DATE FROM SERVER
    SELECT CURDATE() ## LOCAL COMPUTER DATE
```

```sh
    SELECT CURRENT_TIME(); ## TIME FROM SERVER
    SELECT CURTIME() ## LOCAL COMPUTER TIME
```

```sh
    SELECT CURRENT_TIMESTAMP(); ## DATETIME FROM SERVER
    SELECT CURRENT_TIMESTAMP; ## DATETIME FROM SERVER
    SELECT NOW() ## LOCAL COMPUTER DATETIME
    SELECT SYSDATE() ## LOCAL COMPUTER DATETIME
```

INTERVAL &mdash;

```sh
    SELECT NOW(), NOW() - INTERVAL 1 YEAR; # MONTH, DAY, HOUR, MINUTE, SECOND AND MICROSECOND
```

LAST DAY

```sh
    SELECT NOW(), LAST_DATE(NOW());
    SELECT NOW(), LAST_DATE(CURRENT_DATE());
    SELECT NOW(), LAST_DATE(CURDATE());
    SELECT NOW(), LAST_DATE(CURRENT_TIMESTAMP());
```

DATE FORMAT

```sh
    SELECT NOW(), DATE_FORMAT(NOW(), '%y-%m-01');
```

DATE SUB

```sh
    SELECT DATE_SUB(NOW(), INTERVAL 10 DAY);
    SELECT SUBDATE(NOW(), INTERVAL 10 DAY);
```

```sh
    SELECT column, DAY(datecol|time) FROM tablename; # DAYNAME, MONTH, MONTHNAME, YEAR, HOUR, MINUTE and SECOND
```

BETWEEN AND

```sh
    SELECT column FROM tablename WHERE YEAR(datecol|time) BETWEEN val AND val;
```

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
