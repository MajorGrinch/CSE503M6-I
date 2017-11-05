## What is this repo for
This is the repo for my CSE 503 Module 6 individual

## Why doesn't the phpinfo.php output the diagnostic page of server
In my opinion, I think the PHP need a "Document Root" to provide service. As we all know, when we look through settings in Apache, we always meet the "Document Root", which is the directory served by php. In previous modules, we have setted the "Document Root" to "/var/www/html", thus leading to php serves only this directroy on port 80. When we access the "phpinfo.php" in the "static" directory through node js, the php file lack php running environment which could allow it to execute, so we can only download it.