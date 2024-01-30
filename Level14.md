
## Level 14 (Live LFI)

 - We will work with the site's URL: first, we will request the PHP server to read the content of the 'solution.php' file, convert it to base64 format, and then return this base64-encoded content as a response. Try this:
 
       `https://lfi.warchall.net/index.php?lang=php://filter/convert.base64-encode/resource=solution.php`
 - Afterwards, we will decode what we have obtained. You can use the website [https://www.base64decode.org/](https://www.base64decode.org/) for this. Once decoded, you will get the solution.
