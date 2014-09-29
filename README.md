harjutus-9
==========
<!DOCTYPE HTML>
<html>
   <head>
    <title>Harjutus9</title>
    <meta http-equiv="Content-Type" content="text/html;
    charset=utf-8">
    <title>PHP põhitõed</title>
   <?php
        function bg_color($value) {
          return $value;
        }

        $color = bg_color("red");
      ?>
      <style>
      body {
        background-color: <?php echo $color; ?>;
      }

      </style>
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
          function say_hello_to($person) {
            echo "Tere {$person}!<br>";
          }
          say_hello_to('Aile');
        ?>
      <h3>Väärtuse tagastamine</h3>
        <?php
          function add($number1, $number2) {
            $sum = $number1 + $number2;
            echo 'Summaks on ' . ($number1 + $number2);
          }
          add(5, 8);
          echo "<br>";
          $result = add(6, 5);
          echo $result;
        ?>
      <h3>Mitme väärtuse tagastamine</h3>
      <ul>
        <?php
          function calculate($nr1, $nr2) {
            $plus = $nr1 + $nr2;
            $minus = $nr1 - $nr2;
            return array($plus, $minus);
          }
          $result_array = calculate(10, 5);
          echo "<li>Numbrite summa on {$result_array[0]}</li>";
          echo "<li>Numbrite vahe on {$result_array[1]}</li>";
        ?>
      </ul>
      <ol>
        <?php
          function calculate2($nr1, $nr2) {
            $plus = $nr1 + $nr2;
            $minus = $nr1 - $nr2;
            return array($plus, $minus);
          }
          list($plus, $minus) = calculate2(100, 50);
          echo "<li> summa on {$plus}</li>";
          echo "<li>vahe on {$minus}</li>"; 
        ?>
      </ol>

   </body>
</html>
