# This code guides your web server to serve up the React app in CPanel hosting.

Follow the steps below to get your site up and running.

- Create .htaccess file in the public folder.
- Copy the code below into the .htaccess file.

`<IfModule mod_rewrite.c>
  RewriteEngine On
  RewriteBase /
  RewriteRule ^index\.html$ - [L]
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-l
  RewriteRule ^.*$ /index.html [QSA,L]
</IfModule>`

This code will configure the server to serve the index.html file and make sure React Router is working correctly.