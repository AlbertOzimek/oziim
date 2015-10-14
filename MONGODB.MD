# How to create back-end tier

## 1.) Create backend instance

1. Go to google cloud platform
2. Create project
3. Create INSTANCE back-end
4. SSH to the instance

## 2.) SSH to the instance

### Update packages and install MongoDB. When asked if you want to continue, type 'Y'.

sudo apt-get update
sudo apt-get install mongodb

### The MongoDB service started when you installed it. You must stop it so you can change how it runs.

sudo service mongodb stop

### Create a directory for MongoDB and then run the MongoDB service in the background on port 80.

sudo mkdir $HOME/db ; sudo mongod --dbpath $HOME/db --port 80 --fork \
--logpath /var/tmp/mongodb