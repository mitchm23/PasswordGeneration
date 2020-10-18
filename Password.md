<!DOCTYPE html>
<html lang="en-us">
  <head>
    <link rel="stylesheet" href="Password.css">
    <meta charset="UTF-8">
    <title>My First Function</title>
  </head>
  <body>
<button class="box" type="button" onclick="pass(this)">Click here for a random password!
</button>

    <script>


    

// when this function is activated, it will generate a random password from string 'char'
    function pass(len){
      var char = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890!@#$%^&*()'
      var pwd = " ";

      
      
      
// using charAt, and Math.random, we are able to return a random character from string 'char'. Using the for loops parameters, it will continue to return a string of characters until 8 has been met.
      for(var i = 0; i<8; i++){
     pwd += char.charAt(Math.floor(Math.random() * char.length));

      }
      // password will reside in console
      console.log(pwd);
      alert("Check the console for your new password!")
    }
    


    


    </script>

  </body>
</html>
