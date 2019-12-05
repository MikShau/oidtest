# oidtest
Used as a test client for the Gluu OpenID Identity provider.
it is a nodejs - express module that attempt to authenticate with the Gluu server using an implicit flow.

On a server with node and npm installed, clone to a new directory and npm install. If no errors, npm start. 
app is accessed on port 3000. modify test.html to fit the client definitions in the gluu server and test by:

http://<node app name or ip>:3000/test.html
The code will contact the gluu server and display a page with info.
click the button to authenticate.
