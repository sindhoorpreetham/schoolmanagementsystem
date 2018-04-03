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

Finally, run the command "mongrel_rails start".This would start the server and it will be accessible at http://localhost:3000.


# Installation in Ubuntu :
Step 1: Install RVM, Ruby and RubyGems

Run the following commands in terminal.

sudo apt-get install libreadline-gplv2-dev gnupg2 libmysqlclient-dev mysql-server curl

gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3

\curl -sSL https://get.rvm.io | sudo bash -s stable

source /etc/profile

rvm install 1.8.7

rvm use 1.8.7@global && gem uninstall rake

rvm use 1.8.7

rvm rubygems 1.3.7 --force

Step 2: Setup
Extract the ZIP archive and save to a directory.

Run the command "gem install bundler" to install Bundler gem.

Run the command "bundle install --local".

Update the MySQL database details in config/database.yml (under "development:")

Open Terminal and navigate to Fedena source. Run the command "rake db:create". This will create the required database.

Create the database from your Database manager.

Finally, run the command "script/server".This would start the server and it will be accessible at http://localhost:3000


