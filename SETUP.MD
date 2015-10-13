# Initial setup

Go to:
https://console.developers.google.com/project

Create Project

Create virtual VM

micro
ubuntu 1004

call it front-end

Go to:
https://console.developers.google.com/project/splendid-alpha-109619/compute/instances
and ssh to the front-end

# Update packages and install git, Node.js and npm. When asked if you want to continue, type 'Y'.

sudo apt-get update
sudo apt-get install git nodejs npm

# Clone the sample application and install application dependencies.

git clone https://github.com/aozimek/todomvc-mongodb.git
cd todomvc-mongodb; npm install

# Start the todo web application. Note: The IP addresses below are internal IPs for communication between servers. You can find these IP addresses on each server’s details page.

nohup nodejs server.js --be_ip 10.240.0.2 --fe_ip 10.240.0.3 &

# After you enter the final command, click Done and then confirm that you want to leave the page to close the SSH browser window.







----------------

# Istall and run the back-end database

# Enter these commands to install and run MongoDB. You can use the keyboard to copy and paste each command line. Click Done when you finish entering all the commands to close the SSH window.

# Update packages and install MongoDB. When asked if you want to continue, type 'Y'.
sudo apt-get update
sudo apt-get install mongodb
# The MongoDB service started when you installed it. You must stop it so you can change how it runs.
sudo service mongodb stop
# Create a directory for MongoDB and then run the MongoDB service in the background on port 80.
sudo mkdir $HOME/db ; sudo mongod --dbpath $HOME/db --port 80 --fork --logpath /var/tmp/mongodb
# After you enter the final command, click Done and then confirm that you want to leave the page to close the SSH browser window.



# Deploying the app:
appcfg.py -A malpaozim-oziim update app.yaml



To do:

https://console.developers.google.com/project

oziim standard box
malpaozim oziim micro
make the ozmex run on the micro box
malpaozim to 






