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
    
    
 
    
    



## Ref
https://www.geeksforgeeks.org/how-to-protect-against-sql-injection-attacks/?ref=rp
