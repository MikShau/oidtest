# oidtest
Used as a test client for the Gluu OpenID Identity provider.
it is a nodejs - express module that attempt to authenticate with the Gluu server using an implicit flow.

On a server with node and npm installed, clone to a new directory and npm install. If no errors, npm start. 
app is accessed on port 3000. modify test.html to fit the client definitions in the gluu server and test by:

http://<node app name or ip>:3000/test.html
The code will contact the gluu server and display a page with info.
click the button to authenticate.

Installation
Ref: https://www.gluu.org/blog/openid-connect-implicit-client/

1: install the nodejs code in this repository on a suitable machine that resides on the same network as the gluu server.

git clone https://github.com/MikShau/oidtest.git

npm install
npm start

2: Define client on Gluu server as follows:
Parameter
Value
Client Name	Implicit Test Client
Application Type	Web
Pre-Authorization	Enabled
Subject Type	public
Scopes	email, openid and profile
Response Types	id_token, token
Grant Types	implicit
Redirect Login URIs	https://localhost/login-callback.html

3: Edit test.html as appropriate

4: Test

