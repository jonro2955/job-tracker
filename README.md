# Job Tracker

Job Tracker is a full-stack PostgreSQL/Express/React/Node (PERN) application that allows job seekers to save and track their personal job application data.

This is a personal project which I created to learn and apply full stack web development technologies while building something that could be useful in my day to day life.

## Tools Used:

<ul>
<li>Create-React-App</li>
<li>PostgreSQL</li>
<li>Express Server</li>
<li>Node.js</li>
<li>Auth0 SDK</li>
<li>Bootstrap</li>
<li>NPM</li>
</ul>

## How to run this app locally:

### 1. Set up PSQL locally:

<ol>
  <li>Install PSQL on your local computer. For full intructions on installing the PSQL database, visit the offical PSQL website: https://www.postgresql.org/</li>
  <li>Open the PSQL shell and login to PSQL on your local system.</li>
  <li>Create a new PSQL database called "jobtracker". </li>
  <li>Copy the SQL code in the job-tracker-server/schema.sql file and paste it in as commands into the PSQL shell. This is required to set up the database tables needed by the application. </li> 
  <li> In the job-tracker-server/main/db.js file, replace the code with login info for your own local PSQL database. </li>
</ol>

### 2. Set up Auth0:

Auth0 is a cloud based authentication SDK that makes it easy for developers to authenticate users using email or Google open authentication protocols. 

In order to run the Job Tracker app, you need to follow the instruction on the following link to create an account and register your application:  
https://auth0.com/docs/libraries/auth0-single-page-app-sdk. 

Then you need to edit the job-tracker-client/src/utils/authConfig.js file with the Client ID abtained from your Auth0 app registration.

### 3. Start the apps:

Download or git-clone the project files to your local system.

CD into both the client and server directories in separate terminal windows.

In each window, install the dependencies, then run the applications.

#### 1st window

`cd job-tracker-server`  
`npm install`  
`npm start`  
(runs server at localhost:5000)  

#### 2nd window

`cd job-tracker-client`  
`npm install`  
`npm start`  
(runs react app at localhost:3000)  
