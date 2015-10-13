ozimx.tk

# Cloud Repository URL
https://source.developers.google.com/p/ozimex1984/

# Cloning the project

gcloud init
gcloud source repos clone default <local-directory>
cd <local-directory>
git push -u origin master

gcloud init
gcloud source repos clone default <local-directory>
cd <local-directory>
git push -u origin master


# Getting started with Node.js on Google Cloud Platform

This repository is the complete sample code for the [Node.js Getting Started on Google Cloud Platform](http://cloud.google.com/nodejs/getting-started) tutorials. Please refer to the tutorials for instructions on configuring, running, and deploying these samples.

The code for the samples is contained in individual branches on this repository.

Tutorial | Branch
---------|-------
[Hello world](https://cloud.google.com/nodejs/getting-started/hello-world) | [1-hello-world](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/1-hello-world)
[Structured data](https://cloud.google.com/nodejs/getting-started/using-structured-data) | [2-structured-data](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/2-structured-data)
[Cloud Storage](https://cloud.google.com/nodejs/getting-started/using-cloud-storage) | [3-binary-data](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/3-binary-data)
[Authenticating users](https://cloud.google.com/nodejs/getting-started/authenticate-users) | [4-auth](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/4-auth)
[Logging app events](https://cloud.google.com/nodejs/getting-started/logging-application-events) | [5-logging](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/5-logging)
[Using Cloud Pub/Sub](https://cloud.google.com/nodejs/getting-started/using-pub-sub) | [6-pubsub](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/6-pubsub)
[Deploying to Google Compute Engine](https://cloud.google.com/nodejs/getting-started/run-on-compute-engine) | [7-gce](https://github.com/GoogleCloudPlatform/nodejs-getting-started/tree/7-gce)

## Contributing changes

* See [CONTRIB.md](CONTRIB.md)


## Licensing

* See [LICENSE](LICENSE)

Deploy to git:
git push -u origin master



gcloud init

Deploy to google cloud:

gcloud preview app deploy app.yaml --set-default


Testing url:
https://malpaozim-oziim.appspot.com
http://localhost:8080/
ozimex.tk

npm start


sass --watch main.scss:main.css


To do:
Check how to deploy the code without deploying the node_modules


https://www.npmjs.com/package/gcloud



Install and run the back-end database

Enter these commands to install and run MongoDB. You can use the keyboard to copy and paste each command line. Click Done when you finish entering all the commands to close the SSH window.

Update packages and install MongoDB. When asked if you want to continue, type 'Y'.
sudo apt-get update
sudo apt-get install mongodb
The MongoDB service started when you installed it. You must stop it so you can change how it runs.
sudo service mongodb stop
Create a directory for MongoDB and then run the MongoDB service in the background on port 80.
sudo mkdir $HOME/db ; sudo mongod --dbpath $HOME/db --port 80 --fork --logpath /var/tmp/mongodb
After you enter the final command, click Done and then confirm that you want to leave the page to close the SSH browser window.




