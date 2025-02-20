[![RDBMS](https://img.shields.io/badge/mySQL_lessons-000?style=for-the-badge&logo=ko-fi&logoColor=white)](#)

> I'm Zaw Linn Tun a Frontend Web Developer on [Zaw Linn - Vlog](https://www.youtube.com/@zawlinn-vlog). :heart:

<!-- #### PROJECT SIMPLE &mdash; -->

<!-- ![PROJECT_IMG](./assets/img/sample.png) -->

<br>

### INSERT DATA &mdash;

```sh
    INSERT INTO tablename (column_name, column_name, ...) VALUE ('string', int, etc...);
```

or

```sh
    INSERT INTO tablename (column_name, column_name, ...) VALUES ('string', int, etc...), ('string', int,etc...),('string', int, etc...);
```

or

```sh
    INSERT INTO tablename VALUE ('string', int, etc...);
```

or

```sh
    INSERT INTO tablename VALUES ('string', int, etc...),('string', int, etc...),('string', int, etc...);
```

<hr/>
<br/>

### GET ALL DATA FROM DATABASE &mdash;

```sh
    SELECT * FROM tablename;
```

or

```sh
    SELECT column_name, column_name, etc... FROM tablename;
```

or

```sh
    SELECT * FROM tablename WHERE condition AND condition;
```

or

```sh
    SELECT column_name, column_name, etc. FROM tablename WHERE condition AND condition;
```

<hr/>
<br/>

PULL OUT NO MULTIPLE VALUEs &mdash;

```sh
    SELECT DISTINCT column_name FROM tablename;
```

or

CONCAT &mdash;

```sh
    SELECT CONCAT (column_name, column_name, ...) FROM tablename;
```

CONCAT_WS &mdash;

```sh
    SELECT CONCAT_WS(' - ', column_name, column_name, etc...) FROM tablename;
```

SUBSTRING &mdash;

```sh
    SELECT SUBSTRING(column_name, start, length) FROM tablename;
```

or

```sh
    SELECT SUBSTR(column_name, start, length) FROM tablename;
```

ALIAS (NICK NAME) &mdash;

```sh
    SELECT column_name AS alias_name FROM tablename;
```

REPLACE &mdash;

```sh

    SELECT REPLACE(column_name, old_letter, new_letter) AS alias_name FROM tablename;
```

UPPER, LOWER &mdash;

```sh
    SELECT UPPER/LOWER(column_name) FROM tablename;
```

<hr/>
<br/>

#### CONDITIONs AND, OR, NOT &mdash;

##### Operators in the WHERE clause

= &nbsp; &nbsp; equal

\> &nbsp; &nbsp; Greater Than

\< &nbsp; &nbsp; Lessthan

\>= &nbsp; &nbsp; Greaterthan or Equal

\<= &nbsp; &nbsp; Lessthan or Equal

<> &nbsp; &nbsp; NOT Equal, Note: In some versions of `SQL` this operator may be written as `!=`

`BETWEEN` &nbsp; &nbsp; Between as a certain range

`LIKE` &nbsp; &nbsp; Search for a pattern

`IN` &nbsp; &nbsp; To Specify multiple possible values for a cloumns

<br/>

```sh
    SELECT * FROM tablename WHERE condition1 AND condition2 AND condition3,...;
```

OR

```sh
    SELECT * FROM tablename WHERE condition1 OR condition2 OR condition3,...;
```

OR AND NOT &mdash;

```sh
    SELECT * FROM tablename WHERE condition1 OR condition2 AND NOT condition3,...;
```

BETWEEN &mdash;

```sh
    SELECT * FROM tablename WHERE column_name BETWEEN num AND num;
```

IN &mdash;

```sh
    SELECT * FROM tablename WHERE column_name IN ('string', 'string',...);
```

NOT IN &mdash;

```sh
    SELECT * FROM tablename WHERE column_name NOT IN ('num', 'num',...);
```

LIKE &mdash;

```sh
    SELECT * FROM tablename WHERE column_name LIKE pattern;
```

#### PATTERNs &mdash;

- %a &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; END word with `a`.
- a% &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; START word with `a`.
- %or% &nbsp; &nbsp; &nbsp; Any word but must include `or` letter in it;
- \_a% &nbsp; &nbsp; &nbsp; Any word but second letter must be `a`;
- a\_% &nbsp; &nbsp; &nbsp; Start with `a` but must be at least 2 letters;\
- a\_%\_% &nbsp; &nbsp; &nbsp; Start with `a` but must be at least 3 letters;\
- a%o &nbsp; &nbsp; &nbsp; Start with `a` and end with `o`

<br />

```sh
    SELECT * FROM tablename WHERE column_name LIKE 'a_%_%';
```

<hr/>
<br/>

### CALCULATE FUNCTIONs &mdash;

COUNT(), AVG(), SUM(), MIN() and MAX()

```sh
    SELECT COUNT(column_name) FROM tablename ;
```

or

```sh
    SELECT * FROM tablename WHERE column_name = (SELECT MIN(column_name) FROM tablename);
```

<hr/>
<br/>

ORDER &mdash;

```sh
    SELECT * FROM tablename ORDER BY column_name ASC|DESC;
```

or

```sh
    SELECT column_name, column_name, etc. FROM tablename ORDER BY num;
```

<hr>
<br/>

LIMIT Clause &mdash;

```sh
    SELECT column_name, column_name, etc. FROM table_name WHERE condition LIMIT num;
```

or

```sh
    SELECT column_name, column_name, etc. FROM table_name WHERE condition LIMIT num ;
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
