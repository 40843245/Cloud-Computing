# XSS (Cross-site Scripting) attack
## Intro
XSS attack refers to an attack that injects a code in html file.

Recall that 
1. to develope a website, we have to use html, php, and JS etc.
2. The .html file can execute JS code either in the attribute of a html tag or in a "<script>" tag.

  Consider the following examples.
  
              
    <!DOCTYPE html5>
  
    <html>
   
    </html>
  
    <body>
        <button onclick="alert("1");">Submit</button>
    </body>
      
  and 
    
    <!DOCTYPE html5>
  
    <html>
      <script> 
        function Notify()
        {
          alert("1");
        }
      </script>
    </html>
  
    <body>
        <button onclick="Notify();">Submit</button>
    </body>

The above two examples are equivalent. When you click a button which is texted "Submit", then the alert("1") was invoked.
  
If one injects malicious code (such as look at cookies of your webbrowser), Wow it scares me.
  
Such this attack is called XSS attack.

## Category
  
There are two fundamental XSS attack.
  
  1) Reflected XSS
  
  2) Stored XSS
  
### Reflected XSS
  
  ![image](https://user-images.githubusercontent.com/75050655/228729451-cf8bc7e6-8510-4480-9b50-1bcd593951fe.png)
  
### Stored XSS
  
  ![image](https://user-images.githubusercontent.com/75050655/228729556-b3143b84-5fd1-4c15-aa59-01895933744c.png)

### DOM based XSS
  
Its instance is reflected and stored.
  
## XSS attack v.s SQL injection attack
  
XSS attack refers attacks to insert malicious code in html.
  
SQL injection attack refers attacks to insert a or some commands in SQL statement, to successful login without correct password.
  
  
  
## Ref
  
What is XSS?
  
https://www.geeksforgeeks.org/what-is-cross-site-scripting-xss/
  
  
XSS attack v.s SQL injection attack
https://www.geeksforgeeks.org/difference-between-xss-and-sql-injection/?ref=rp
