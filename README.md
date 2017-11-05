## What is this repo for
This is the repo for my CSE 503 Module 6 individual

## Why doesn't the phpinfo.php output the diagnostic page of server
In my opinion, I think the PHP need a "Document Root" to provide service. As we all know, when we look through settings in Apache, we always meet the "Document Root", which is the directory served by php. In previous modules, we have setted the "Document Root" to "/var/www/html", thus leading to php serves only this directroy. When we access the "phpinfo.php" in the "static" directory, the file lack running environment which could allow it to execute, so we can only download it.  
But when I execute the command "php -S 0.0.0.0:8000 -t ./" in the "static" directory, then I can access the "phpinfo.php" in the node.js http server.