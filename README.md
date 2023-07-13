# WanderLust🎒

## Description
A full stack website that uses MERN stack for tour bookings.

## Steps to run locally :
1) `Clone/download` the repository
2) Do `npm install` in both client and server folders (since they both have separate set of node modules).
  May face few errors , because few of node modules that I used may have been deprecated by the time of your use . So I suggest you to fix those module errors first , through suggested methods available online at your time.
3) Create a .env file in server folder and fill all the following fields  : `PORT` , `CLIENT_URL='http://localhost:3000'` , `MONGODB_URL` , `USER_TOKEN_KEY` , `ADMIN_TOKEN_KEY` . For token keys use any two random hashed values (one for each) (you can generate online or using node/javascript libraries) 
4) Do `node seeder.js` in server folder to upload all data present in **Data folder** to **Mongodb database** (the app runs by fetching data from mongo database)
5) To access admin : add a admin folder in mongodb database along with added data in previous step , the fields are `username` and `password` . Fill any username you like , the password stored in database is encrypted using hashing at a particular cost factor(refer to code to know how much) , so hash your preferred password in [bcryptonline](https://bcrypt.online/) website and add the hashed value in password field of admin document of database , so it can decrypt and verify for correct password when you want to login. 
6) Now do `npm start` or `npm run dev` first in server terminal , and same next in client terminal.

   Website should be up and running !


## Possible improvements :
1) get rid of bootstrap and only focus on pure HTML and CSS
2) implement a payment gateway for bookings
3) implement forgot password feature
4) implement email notifications to customer on successful booking , or successful creation of account

