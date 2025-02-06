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

### Numberic DATA TYPEs &mdash;

#### STRING DATA TYPEs &mdash;

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
