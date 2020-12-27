# LMS
## About the project
A simple Library Management System using **MongoDB, Node js, Express, jquery**.
CRUD services have been included for books and users.The user can belong to either **Admin or Customer** category.
> - **Admin role** includes Add/Update Book inventory,Add another admin/user,force delete users(in the sense who still have books pending to be returned) 
or raise a flag on the user for any violations. 
> - **Customer role** includes renewal of books(increases for every 7 days),return book,update user account and delete their account if no books are in due.
>   
Template engine used: **EJS**.  
MongoDB is used with Mongo Atlas and hosted in the cloud.All the  environment variables are available in **.env** file.  
## Running the project
> - To run the project locally, grab the code from the github repository into the local machine,navigate to that folder and install all dependencies(refer the **app.js** file).
Type the command **npm start**/**npm run dev** in your terminal..
> - To see a demo of the working project already deployed in heroku app just use this url [LibSys](https://library-system-manager.herokuapp.com/)


## Few more add-ons to work with the project(only for ease of working)
> - To login as a admin you can either do a admin signup from the landing screen (But you will need a admin secret to go ahead.)This configuration variable is set in 
the **.env** file. This additional attribute is used to reinforce different schema for customer and admin.For simplicity it is set to **admin**
> - To login as a customer just do a user signup and interact with the model.

## On a final note
This app is created in heroku and pushed from the local cli.So none of the additional commits from the local repository will be visible to you.This repository in github is used
to contain the code that is deployed, so everything is dumped in a single commit and this repo will not have a environment setup in it.If you want to clone the demo app in heroku in your local machine use this
**heroku git:clone -a library-system-manager**

