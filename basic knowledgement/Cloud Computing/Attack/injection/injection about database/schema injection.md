# schema injection
## Level 
easy (I thinl it is easy)
## Prequisite
schema
## Review
If you know what is schema. Don't worry I will review it.

Recall that there are a few database to store the important information (such as the current user name of the DBMS) in each DBMS (Database Management System).

The following figure illustrate the database which stores important information.

![image](https://user-images.githubusercontent.com/75050655/232259290-24c8c16c-6d3b-4ed9-bd68-ad0ae7bcaf7f.png)

Schema describes the structure of the table in the database, format of each field, and the relation between each tables.

## Intro

Consider the following situation.

If the attacker can access your schema, then one will know that

    1) structure of the table in the database
    2) format of each field, and
    3) relation between each tables.
    
Furtherly, one can easily to inject them between the SQL command (since one has known the format of each field, making it more easily to know what kind of 

input is valid or invalid.)

For example, an attacker can utilize schema injection to inject thousands of columns onto the database with data of the attacker’s choice. 
