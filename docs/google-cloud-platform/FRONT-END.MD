# How to create front-end tier

## 1.) Create front-end instance

1. Go to google cloud platform
2. Create project
3. Create INSTANCE back-end
4. SSH to the instance

## 2.) SSH to the front-end instance

### Update packages and install git, Node.js and npm. When asked if you want to continue, type 'Y'.

sudo apt-get update
sudo apt-get install git nodejs npm

### Clone application

git clone https://github.com/aozimek/todomvc-mongodb.git
cd todomvc-mongodb; npm install

### Start the todo web application. Note: The IP addresses below are internal IPs for communication between servers. You can find these IP addresses on each server’s details page.

nohup nodejs server.js --be_ip 10.240.0.2 --fe_ip 10.240.0.3 &

