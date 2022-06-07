Contact Form Without a Server Using Angular

Finished contact form using Material without a server
Do you ever need a contact form for your personal website, but don’t want to have to setup a backend server, use SendGrid, Mailchimp, Formspree, to send only a few emails a day? Look no further, you can send emails and log them in a Google Spreadsheet without having to spend any money or time managing, deploying, and creating a backend server.

Overview
In this tutorial, we will be going through the following concepts:

Creating our Google service to send emails
Angular Reactive Forms
Form creation using HTML and CSS and data binding
Pre-requisites
To follow along, you will need to have NodeJS and Angular CLI installed on your computer, and a Google account to send emails.

Creating your Google service to send emails
This was made by using Send Email from a Static HTML Form using Google Apps Mail! repository which goes through the full details on implementing this onto your Google account. Full credit goes to the developers that worked on the project.

Start by making a copy of [this spreadsheet](https://docs.google.com/spreadsheets/d/1ro0xwCDh9ED4dsNWc6IBE3uUU1wukpVhDQOABrMesmY/edit#gid=0) using your Google Account.
Open the Script Editor by clicking “Tools” > “Script Editor”
Uncomment the TO_ADDRESS field and change example@email.net to your email
Save it by clicking “File” > “Manage versions” and typing in a version name
Publish it as a web application by clicking “Publish” > “Deploy as web app…” and select the latest project version
Authorize the application and copy the web application URL
Now that you’re done setting up the script that will handle all the submissions, we can start by creating a form to utilize our created script.

Create a new Angular App and a component
Creating a new Angular application is quite easy using the Angular CLI. Start by opening the Command Prompt or Terminal and creating the application using the Angular CLI. After the application has been created, generate a component (in this case our contact component) to put our forms into. We will be using the Material theme to style our form.

