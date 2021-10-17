# Serverless NOTEPAD

a notepad application where user can add notes and attach images to them

# Functionality of the application

* This application will allow creating/removing/updating/fetching NOTE. 
* Each NOTE can optionally have an attachment image. 
* Each user only has access to NOTES that they has created.

# the applicatiion has two parts a frontend and a backend 

## frontend

The client folder contains a web application that can use the API developed in the project. This frontend works with the serverless application.

## backend

The backend folder contains a serverless application that uses the serverless framework

* The code is split into multiple layers separating business logic from I/O related code.
* Code is implemented using async/await and Promises without using callbacks.

# Authentication
Authentication in this application, is done through Auth0, Which uses asymmetrically encrypted JWT tokens.

* https://auth0.com/blog/navigating-rs256-and-jwks/

# How to run the application

## Backend

To deploy an application run the following commands:

```
cd backend
npm install
sls deploy -v
```

## Frontend

To run the app run the following
```
cd client
npm install
npm run start
```

This should start a development server with the React application that will interact with the serverless NOTEPAD application.

# Postman collection

An alternative way to test your API, you can use the Postman collection that contains sample requests. You can find a Postman collection in this project. To import this collection, do the following.

Click on the import button:

![Alt text](images/import-collection-1.png?raw=true "Image 1")


Click on the "Choose Files":

![Alt text](images/import-collection-2.png?raw=true "Image 2")


Select a file to import:

![Alt text](images/import-collection-3.png?raw=true "Image 3")


Right click on the imported collection to set variables for the collection:

![Alt text](images/import-collection-4.png?raw=true "Image 4")

Provide variables for the collection (similarly to how this was done in the course):

![Alt text](images/import-collection-5.png?raw=true "Image 5")
# capstone-cdnd
