#VotingApp:
The app allows user to vote on different political parties. 


- To create a URLconf in the polls directory, create a file called urls.py
The next step is to point the root URLconf at the polls.urls module
- Creating Models: In our poll app, we’ll create two models: Question and Choice. A Question has a question and a publication date. A Choice has two fields: the text of the choice and a vote tally.

Migrations
When you create a model, it contains essential fields and behaviors of your stored data. To activate a models you add a reference in the settings to say that your app is installed. Now you should use the makemigrations command, Django will know that you’ve made some changes to your models and will store them as a migration.

Then you can use the migrate command will apply those changes to the database. It will also create all necessary database tables you need by reading the Installed_apps settings in the settings.py file. The default ones are: the admin site, authentication system, content types, sessions, messages, and static files. 

Migrations are very useful because they allow you to change and update your databases live so that you don’t lose data and so you don’t need to delete or make new ones. You can also use the sqlmigrate command to return the SQL of your migrations. It just prints it to the screen, not actually running it, which is useful if you want to see what Django is going to do.
