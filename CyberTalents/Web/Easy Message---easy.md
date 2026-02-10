*just normal login page

trying sqlmap  didnot work 

fuzzed >found robots.txt >> 
    User-agent: *
    Disallow: /?source

entered /?source 

<?php

$user = $_POST['user'];
$pass = $_POST['pass'];

include('db.php');

if ($user == base64_decode('Q3liZXItVGFsZW50') && $pass == base64_decode('Q3liZXItVGFsZW50'))
    {
        success_login();
    }
    else {
        failed_login();
}

?>

--
user =Cyber-Talent
pass =Cyber-Talent
--

loged in >

found morse code 
..-. .-.. .- --. -.--. .. -....- -.- -. ----- .-- -....- -.-- ----- ..- -....- .- .-. ...-- -....- -- ----- .-. ... ...-- -.--.-

translated to 


FLAG(I-KN0W-Y0U-AR3-M0R3)































