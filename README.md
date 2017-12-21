# Windows-herokuPG-setup


Windows users tend to have trouble using heroku psql database because they cannot push their local databases up to the deployed version. This doc will be a tutorial on how to do that.

We will start at ground zero where we make a local database, then create a heroku app, and then we will go from there.


### Make a local psql database:

- Make the db,
- Make a table,
- Insert data into the table,
- check that you can select * from <table_name>


### Make a heroku app and addon the pg database

- create a new app.
- go to the resources tab.
- search for postgres.
- Heroku postgres should pop up.
- Double check that it's postgres Database, not Ivory or some other variant.


### clone your github project down to your local machine.
##### NOTE: if you don't have a project repo setup yet then stop here and come back when you have your repos setup how you want them. 

- Clone down your project repo.
- Navigate into the dir that holds your server data. (IE if you have a front end repo and back-end repo, navigate into the back-end repo).

- Nothing else at this point, but we'll come back here in a couple minutes


### Connect your github to the herokuap

- Navigate to the deploy tab.
- Click on the second icont option for connecting to git-hub( it's the image of octocar).
- follow the steps to connect you github account to this heroku app.


### download the Heroku CLI installer.

- Windows's install option is a 'Binary installer'. It's just a normal download and install software program.
- Follow all the default setup options.
