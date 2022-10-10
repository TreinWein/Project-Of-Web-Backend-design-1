# Project-Of-Web-Backend-design-1


<?php


    
?>


<!DOCTYPE HTML>

<html lang="pl">


<head>

    <!-- Sposob Kodowania Znakow na Stronie -->
    <meta charset="utf-8"/>

    <!-- Slowa Kluczowe Na Stronie -->
    <meta name="Keywords"
    content="Sneakers,Skeakersy,Buty,Yezzy"/>

    <!-- Autor Strony -->
    <meta name="Author" content="AS"/>

    <!-- Opis Strony -->
    <meta name="Description"
    content="Strona O Butkach Fajnowych"/>

    <!-- Co to jest -->
    <meta http-equiv="X-UA-Compatible"
    content="IE-edge,chrome=1" />


    <!-- Tytul Strony -->
    <title> Buciki </title>

</head>



<body style="background-color: #05516e;">

<div style="position:absolute; top:40%; left:30%;
    height: 100px; widht: 100px;
">
<form action="zaloguj.php" method="POST">

    <label style="color:#d5bb04">Login</label>
    <input type="text" placeholder="Type Login: " 
    name="log" required="required"></input> <br>

    <label style="color:#d5bb04">Pass.</label>
    <input type="password" placeholder="Type Password: "
    name="pass" required="required"></input> <br>

    <input type="submit" value="Log in"></input>


<?php

    if(isset($_SESSION['log_error'])){
        echo $_SESSION['log_error'];


        unset($_SESSION['log_error']);

    }


?>

</form>
</div>


<div style="position: absolute; top: 40%; left: 70%;">


<form action="POST">

    <label style="color:#d5bb04"> Podaj Login </label>
    <input type="text" placeholder="Login Rejestracja"
    name="Rlogin"> </input><br>

    <label style="color:#d5bb04"> Podaj Email </label>
    <input type="text" placeholder="E-mail Rejestracja"
    name=Remail> </input><br>

    <label style="color:#d5bb04"> Podaj Haslo </label>
    <input type="text" placeholder="Haslo Rejestracja"
    name=Rhaslo1> </input><br>

    <label style="color:#d5bb04"> Powtorz Haslo </label>
    <input type="text" placeholder="Haslo Rejestracja"
    name=Rhaslo2> </input><br>

    <label>
    <input type="checkbox" name="regulamin" /> 
        <span style="color:#d5bb04"> Akceptuje Regulamin </span> <br>
</label>


    <input type="submit" value="Wyslij Formularz"> </input>

</form>


</div>



</body>
</html>


