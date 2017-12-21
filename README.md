# Windows-herokuPG-setup


Windows users tend to have trouble using heroku psql database because they cannot push their local databases up to the deployed version. This doc will be a tutorial on how to do that.

We will start at ground zero where we make a local database, then create a heroku app, and then we will go from there.

### Pre-check

- Make sure that psql has been added to your path. Click here to learn how to do that. You may have to close your terminal, restart, and check the path again to make sure it was added and saved.
- If the above was successful, then you should be able to type `psql` in git bash and it should prompt you for your password. 
- Note that by default, psql will try to log in using the name of whichever account you are logged into. If that's the case, then you might not be able to login because the default user is postgres. You can login into psql as a different user by typing `psql -U <username>` where your username goes inbetween the <>. Typically, the default user in psql is postgres, so you will most likely be typing `psql -U postgres`. The `-U` is a quick flag that stands for username.
- Also note that this is the password that you gave when you first installed psql. If you want to change your password then click here to learn how.


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
