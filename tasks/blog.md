# c

## Zadanie

Zadanie znalezione w internecie.
Pliki potrzebne do zadania: [task-01.zip](https://github.com/s0bieskii/junior-java-guide/src/task-01.zip)

```
Java must be used to implement the task. The used database system can be chosen freely. The
sample data comes from a mySQL database. Please do not use any prefabricated frameworks.
Task 1: Please create a small program that provides the functionality for a blog with the given
data. The frontend does not need to be created, only the endpoints need to be accessible.
Especially think about structuring the code. Please explain your code in writing (comments or free
text) and share your decisions.
Demodata for Task 1
CREATE TABLE `user` (
`userid` INT NOT NULL AUTO_INCREMENT PRIMARY KEY ,
`username` VARCHAR( 45 ) NOT NULL ,
`password` VARCHAR( 45 ) NOT NULL ,
`permission` VARCHAR( 45 ) NOT NULL ,
`readonly` VARCHAR( 45 ) NOT NULL
) ENGINE = InnoDB;
CREATE TABLE `blog` (
`id` INT NOT NULL AUTO_INCREMENT PRIMARY KEY ,
`text` TEXT NOT NULL ,
`userid` INT NOT NULL
) ENGINE = InnoDB;
Endpoints
- list
http://domain/blog
- login
http://domain/blog?action=login&user=admin&password=admin
- new entry
http://domain/blog?action=new&text=testtext
- new user
http://domain/blog?
action=new_user&username=test&password=test&permission=superuser&readonly=yes
- delete entry
http://domain/blog?action=delete&id=1
Page of1 2
Topic Databases
Given is a mySQL dump of a database table (task.sql file). This contains offers for mobile
homes (motorhomes) at different locations all over the world. The contained data are only
an excerpt of a database. A data volume of about 5 million records is expected, which are
constantly updated, deleted and rewritten.

Detailed information about the columns:
• city, city_en. city_fr :
• city name in German, English and French
• country, coutnry_en, country_fr :
• country name in German, English and French
• extra, extra2, extra3
• Extras that can be added if needed
• The column contains the following data: Name, price in Euro and price in US dollars.
The data are separated by a semicolon separated from each other.
• insurance, insurance2, insurance3
• Insurances that can be added
• The column contains the following data: Name, price in Euro and price in US dollars.
The data are separated by a semicolon.
The following data are regularly retrieved from the database :
• All city/country combinations where motorhomes are offered, grouped by the different
languages.
• All offers (motorhome + price) for a city, where the city name must be must be
independent of the language:
• Example: Cologne or Köln must give the same results.
• The data must be sorted by price.
• All offers (city, country, RV and price) for a specific RV, grouped by country and city,
sorted by price.
• All offers (city, country, RV and price) in a given price range. The currency is freely
selectable. The data should be sorted by price.
Task 2a
Briefly describe where you see problems when working with this table and how these
problems could be solved.
Task 2b
What would be considered in the choice of data types for each column ?
Task 2c
What is meant by an "index" on a table and what should be considered when indexing ?
What indexes would you set in the given example ?
Task 2d
Explain briefly what "foreign keys" are, when they should be used and when they should
not be used! Would you use foreign keys in the example ? Please give reasons for your
answer.
```