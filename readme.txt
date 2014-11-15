To run this application, start your mongo server & do the following from the command line:
bower install
npm install
nodemon server.js

 you also need to have mongodb running on your mac. 


 only tested on mac. 



on file server/controllers/user.js     it's first encrypting the text for password and then saving it in the db. 

You can search for followign lines of code 


  userData.salt = encrypt.createSalt();
  userData.hashed_pwd = encrypt.hashPwd(userData.salt, userData.password);



