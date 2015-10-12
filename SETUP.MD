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

git clone https://github.com/GoogleCloudPlatform/todomvc-mongodb.git
cd todomvc-mongodb; npm install

# Start the todo web application. Note: The IP addresses below are internal IPs for communication between servers. You can find these IP addresses on each server’s details page.

nohup nodejs server.js --be_ip 10.240.0.2 --fe_ip 10.240.0.3 &

# After you enter the final command, click Done and then confirm that you want to leave the page to close the SSH browser window.






