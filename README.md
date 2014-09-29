harjutus-9
==========
<!DOCTYPE HTML>
<html>
   <head>
    <title>Harjutus9</title>
    <meta http-equiv="Content-Type" content="text/html;
    charset=utf-8">
    <title>PHP põhitõed</title>
   </head>
   <body>
   		<h2>Funktsiooni defineerimine</h2>
   		<h3>Argumendita funktsioon</h3>
        <?php
          function say_hello() {
            echo 'Minu esimene funktisoon!<br>';
          }
          say_hello();
        ?>
      <h3>Argumendiga funktsioon</h3>
        <?php
          $person = "Aile";
          function say_hello_to($person) {
            echo "Tere {$person}!<br>";
          }
          say_hello_to($person);
        ?>
   </body>
</html>
