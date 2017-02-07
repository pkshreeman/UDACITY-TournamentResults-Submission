# UDACITY FSND
## Tournament Results Project
### Objective
1. Operate a database using Postgres
2. Write python program to manipulate the database using the psycopg2 package
3. Develop routines to pass tests of swiss-style of players' pairings by keeping track of who is winning, and properly matching the players by their ranking.

Provided four files:
- readme.md:  This file that you are reading...
- tournament.py : A python file that incorporates the routines necessary to pass the testing routine
- tournament_test.py: A python file that was provided by UDACITY for testing purposes.
- tournament.sql: A sql file to create the initial database for the testing routines.

###What do you need?

The database that I am using is Postgres 9.3.15.  [Install Postgres](https://wiki.postgresql.org/wiki/Detailed_installation_guides).
The programming language that I currently use is python 
[Install Python](https://www.python.org/downloads/)

If you are using Linux or MacOS, you should already have Python installed.  However, I used Python 3.5 with Anaconda install (Python 3.5.2 :: Anaconda 4.2.0) so if you have a different version, it is possible to see some errors.  To find out, type python -V at terminal.  Make sure that you type capital "V" for the version.

There is also standardized method of using virtualized machine using vagrant and Virtualbox with ready-made files at https://github.com/udacity/fullstack-nanodegree-vm 
- [Install Virtualbox](https://www.virtualbox.org/)
- [Install Vagrant](https://www.vagrantup.com/)

For comprehensive guide on creating this virtual standardized server, check out the documentation provided by Udacity:  [Guide](https://docs.google.com/document/d/16IgOm4XprTaKxAa8w02y028oBECOoB1EI1ReddADEeY/pub?embedded=true)

###Now what?

Assuming that you are at command prompt at the same folder as the files, type ```psql``` to enter the Postgres command prompt.  Once there, type ```\i tournament.sql```.  You should see the following output:
```
DROP DATABASE
CREATE DATABASE
You are now connected to database "tournament" as user "XXXXX".
CREATE TABLE
CREATE TABLE
CREATE VIEW
```
Once that is completed, you then exit by typing ```\q``` back to normal command prompt.  Then to run the test, you enter ```python tournament_test.py```  The only output that you will see is the test results. not the SQL results itself.