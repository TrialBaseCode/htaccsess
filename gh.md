RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
// get the admin file take as admin/index.php
RewriteRule ^admin/?$ admin/index.php [L]
// get the counter file take as counter/index.php
RewriteRule ^counter/?$ counter/index.php [L]
RewriteRule ^([^\.]+)$ $1.php [L]

//404 error
ErrorDocument 404 /restaurent/notfound.php

