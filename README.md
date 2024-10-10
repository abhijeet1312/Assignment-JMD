# Assignment Uploader 
A Node.js application that allows users to register, log in, and upload assignments. Admins can review these assignments and accept or reject them.  


## Table of Contents  

- [Installation](#installation)  
- [Usage](#usage)  
- [Features](#features)  


## Installation  

1. **Clone the repository:**  

  
   git clone https://github.com/abhijeet1312/Assignment-JMD.git  
   cd Assignment-JMD
2. **Install dependencies:**
     npm install

## Usage
 1. To start this project on your local computer run the following command on your terminal after moving to the root directory:
    npm start
 
2. ## Environment Variables  
Before running the application, you need to set up the necessary environment variables for it to function correctly. Below are the following  variable:

- **GOOGLE_CLIENT_ID** and  **GOOGLE_CLIENT_SECRET**: This is the client ID and Secret you will receive after registering your application on the Google Cloud Platform for OAuth2. The client ID is essential for enabling Google authentication in your application. To obtain this ID, follow these steps:  

  1. Go to the [Google Cloud Console](https://console.cloud.google.com/).  
  2. Create a new project or select an existing project.  
  3. Navigate to the "APIs & Services" section and click on "Credentials."  
  4. Click on "Create Credentials" and select "OAuth 2.0 Client IDs."  
  5. Follow the setup process, specifying the authorized redirect URIs as required for your application.  
  6. Once your credentials are created, you will see your **Client ID** and **Client Secret**. Copy this value and set it in your 
     environment :
- **SESSION_SECRET**: Variable which holds the session secret of session middleware
- **JWT_SECRET**:Variable which holds the session secret of JWT
- **MONGODB-URI**:Url which connects our server to MongoDB ,we can get this using mongodb compass or atlas
- **PORT**:sample port
## Features   
For **User** Following are the routes
     **"/register"**:Post route to register the User
     **"/loginUser"**:Post route to login the User
     **"/user-assignment"**:Post route to submit the user assginment
     **"fetchadmins"**:Get route to fetch all the admins 
     
   For **Admin** Following are the routes
     **"/registerA"**:Post route to register the Admin
     **"/loginAdminMain"**:Post route to login the Admin
     **"/assignment"**::Get route to fetch all the assignment tagged to logged in Admin
     **"/assignment/:id/accept"**:Post route to accept the particular assignment
     **"/assignment/:id/rejct"**:Post route to reject the particular assignment
      
   

   
    
   
