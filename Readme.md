<h3 style="text-align:center;">Hospital-API</h3>
In a time where a major pandemic has covered all the world we need a system which can track patients data and generate reports for them. This is a very basic API which exactly do this. 

## Basic Features
1. Register Doctor with username, password and name.
2. Login(authenticate) User using passport-local and returns a jwt-token to be to access(authorize) protected routes.
3. After logging-in the doctor can do various things such as : register patient, generate a report of patient, view all reports of a particular patient, filter all the reports by status.
4. Generation of report(protecte by jwt) : A doctor has to enter enter the status for a particular patient and can generate the report according to it.
5. View all reports of a patient(protected by jwt) : A doctor can view all the reports of a patient.
6. View all the reports filtered by status(protected by jwt) : A doctor can view all reports present in database filtered by status.
7. Unit testing integrated.

## How to install and run?
1. Clone this project
2. Start by installing npm and mongoDB if you don't have them already.
3. Run the Mongo Server.
4. Navigate to Project Directory by :
```
cd Hospital-API
```
5. run following commands :
```
npm install 
npm start or node index.js
```


## How to use API (Understanding the end points)? (!!Important in understanding API)
#### Base URL : `http://localhost:8000/api/v1`
#### End Points :
1. Example input : (send name, username, password and confirm-password) <br>
 
## Directory Structure and flow of The Code
This code follows MVC pattern and hence everything is differentiated and well managed:

`/routes` - containes all the routes. <br>
`/routes/api` - containes api files <br>
`/assets` - static js css and image files. <br>
`/controller` - contains functions to connect to different routes. <br>
`/controller/api` - contains functions to connect to different end points of api. <br>
`/model` - to store data in db we need models. <br>
`/config` - contains config files for mongoose, passport or any other configs such as middlewares. <br>
`/test` - contains files to test the code. <br>

Feel free to use and contribute! :)

    
