# SQL injection 
## Intro
SQL injection attack refers attack via injection of SQL command.

Recall that 
    
    SQL command is represented as a string. 
    
With this characteristic, it becomes vulnerable since the attacker can query for specific data and perform some specific operation in SQL.

via input an invalidate text.

Consider the SQL statement as example.

    $name= $_GET['username'];
    $password=$_GET['password'];
    $sql= "SELECT * FROM table1 WHERE username = '".$name."'"." AND password = '".$password."'";
    
 If one inputs in the 'username' field,
 
    hacker // 
  
 then what happens?
 
    Since the // refers a single-line comment in SQL, it will NOT check the password. 
    
    Here, iff the 'username' matches, the condition in where clause will be satisfied, causing expected result.
    
    (It is expected that iff the 'username' and 'password' matches, the condition in where clause will be satisfied.)
    
And what if it is used in login check.

Wow!!! It scares me.

Therefore, prevention of SQL injection attack is very important for anyone.

Before introducing the  prevention of SQL injection attack, let's started with type of SQL injection attack.

## Type
The above section just discuss the core concept of SQL injection and how it works.

In this section, I will discuss the more complex and detailed about SQL injection.

Let's dig in.

There are 4 major SQL injection attack. (thanks to GeeksForGeeks)

    1) Error-based SQLi
    2) Union-Based SQLi
    3) Blind Boolean-based SQLi
    4) Blind Time-Based SQLi
    
 
1. Error-based SQLi: Error-based SQLI obtains information about the database structure from error messages issued by the database server. In rare circumstances, an attacker may enumerate an entire database using only error-based SQL injection.

2. Union-Based SQLi: Union-based SQLI uses the UNION SQL operator to aggregate the results of two or more SELECT queries into a single result, which is subsequently returned as part of the HTTP response.

3. Blind Boolean-based SQLi: Boolean-based SQL Injection works by submitting a SQL query to the database and forcing the application to produce a different response depending on whether the query returns TRUE or FALSE.

(Hint: 

Recall the critical feature in SQL which is similar to C/C++.

Given one expression, if it can determined to true or false, then it will NOT continue to be evaluated for performance.

Such as

In SQL,

WHERE true OR username = '123';

    the condition username = '123' 
    
will NOT be checked.

Equivalently, in C/C++

if(true OR username == '123')

    the condition username == '123' 
    
will NOT be checked.
    
Since it takes a little time to check a condition, with this feature, the attacker can check each conditions is evaluated to true or false. 
    
    (The computer can measure time accurately.)

)

4. Blind Time-Based SQLi:
Time-based SQL Injection works by sending a SQL query to the database and forcing it to wait for a predetermined length of time (in seconds) before answering. The response time will tell the attacker if the query result is TRUE or FALSE
    
## Prevention

    1) Use extensive data Sanitization
    2) Make use of a web application firewall
    3) Patch software on a regular basis
    4) Contextually limit database rights
    5) Monitor SQL statements from database-connected apps in real-time
## Ref
https://www.geeksforgeeks.org/how-to-protect-against-sql-injection-attacks/?ref=rp
