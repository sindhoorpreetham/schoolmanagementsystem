This is a open source School management system based on Ruby on Rails by Foradian, and is now maintained by the open source community.

# Installation in Windows :
Step 1: Install Ruby
Download and install One-Click Ruby Installer for Windows. 
https://dl.bintray.com/oneclick/rubyinstaller/rubyinstaller-1.8.7-p302.exe 

Step 2: Install MySQL
Download and install the "essential" version of the MySQL installer v5.0 
http://downloads.mysql.com/archives/mysql-5.0/mysql-essential-5.0.90-win32.msi
(skip this step if you already have MySQL installed)
Copy libmysql.dll from MySQL bin directory (usually C:\Program Files\MySQL\MySQL Server 5.0\bin) to Ruby bin directory (usually C:\Ruby\bin)

Step 3: Setup
Extract the ZIP/TAR archive and save to a folder (say C:\Test).
Now goto the source directory in the command window.
Run the command "gem install bundler --remote" to install Bundler gem.
Run the command "bundle install --local".
Update the MySQL database details in config/database.yml (under "development:")
Run the command "rake db:create". This will create the required database.
Create the database from your Database manager.
Finally, run the command "mongrel_rails start".This would start the server and it will be accessible at http://localhost:3000
