# Generic-hashed-credential-inputs
example of a simple HTML login form with JavaScript for client-side hashing of the password input before it is sent to the server
Note:

The form uses the onsubmit attribute to call the hashPassword() function, which hashes the password input before the form is submitted.
btoa() method will be used for JavaScript level encryption.
The hashed password is then sent to the server along with the username.
To check the validation of login, you need to match the hashed input with the previous ones that are stored in the database. 
You can achieve this by creating a route in your server side that accepts post request with user name and hashed password. 
Your server will check the hash with the previous ones stored on the database, if matches it will generate a new HTML page with accepted login message, otherwise an generic error message will be sent back.

This is just an example to give an idea of how you can implement client-side hashing of passwords, but in a production environment, it is recommended to use a more secure method of encryption and to also hash on the server side to prevent any tampering with the client side code.



