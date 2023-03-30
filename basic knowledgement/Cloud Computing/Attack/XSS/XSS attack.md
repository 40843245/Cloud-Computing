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
