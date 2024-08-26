<?php

   $connection = mysqli_connect('localhost','root','','iform');

   if(isset($_POST['Submit'])){
      $First_name = $_POST['First_name'];
      $Last_name = $_POST['Last_name'];
      $Email = $_POST['Email'];
      $Contact = $_POST['Contact'];
      $Password = $_POST['Password'];

      $request = " INSERT INTO `iform` (`ID`, `First_name`, `Last_name`, `Email`, `Contact`, `Password`) VALUES (NULL, 'Cristine', 'Tullao', 'Ctullao@yahoo.com', '09085876621', 'ctullao')";     
       mysqli_query($connection, $request);

      header('location:index.html'); 
   if{
   	echo 'Succcessfully Registered';
   }else {
      echo 'something went wrong please try again!';
   }

?>