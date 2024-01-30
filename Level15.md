## Level 15 (Live RFI)

 - For this challenge, we do the same thing as in the previous one, meaning we enter the URL to request the PHP server to read the content of the 'solution.php' file, convert it to base64 format, and then return this base64-encoded content as a response :
 
       `https://rfi.warchall.net/index.php?lang=php://filter/convert.base64-encode/resource=solution.php`
 
 - And then we will decode what we obtained on the site https://www.base64decode.org/fr/ to have the solution 
 
