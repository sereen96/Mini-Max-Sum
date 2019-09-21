<!DOCTYPE html>
<html>
<head>
<title>prime number</title> 
</head>
<body>
<form action ="#.php" method ="post">
number <input type="text" name ="num"><br>
<input type="submit" name="submit">
  
<?php 
  $num = $_POST['num'];
  function primenumber(int $num){
   $countt=0;
     if($num<=1)
      return false ;
   
  for ($i=2;$i<$num;$i++){
   if ($num%$i==0)
      $countt ++;
  }
     
   if ($countt>=1)
     echo("the number is not prime " . $num);
   else 
     echo("the number ia a prime ". $num);

 }
  
 echo( primenumber($num));
?>
</body>
</html>
