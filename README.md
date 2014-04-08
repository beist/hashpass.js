hashpass.js
==========

JavaScript snippet to hash plain text passwords before sending/posting them to validation on servers, so hashing does not have to happen on server side, though making transportation of password-data even over SSL more secure.

Imagine, somehow a man in the middle happens to decrypt the over SSL transported data you transmitted to a service, he could read the password transmitted. Since passwords are (or should be) encrypted in any user database, why not transfering them encypted also, since the first network activity. So everything a man in the middle could read would be the encrypted password hash.
