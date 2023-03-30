# XSS (Cross-site Scripting) attack
## Intro
XSS attack refers to an attack that injects a code in html file.

Recall that 
1. to develope a website, we have to use html, php, and JS etc.
2. The .html file can execute JS code either in the attribute of a html tag or in a "<script>" tag.

  Consider the following examples.
  
              
    <!DOCTYPE html5>
  
    <html>
      <script> 
        function Notify()
        {
          alert("1");
        }
    </html>
  
    <body>
        <button onclick="Notify();">Submit</button>
    </body>
      
  and 
    
    <!DOCTYPE html5>
  
    <html>
      <script> 
        function Notify()
        {
          alert("1");
        }
    </html>
  
    <body>
        <button onclick="Notify();">Submit</button>
    </body>

