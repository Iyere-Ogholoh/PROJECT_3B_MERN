# PROJECT-3B-MERN STACK IMPLEMENTATION

## BACKEND CONFIGURATION

Update Ubuntu

`sudo apt update`

![updating ubuntu](./images/backend-configuration/updating-ubuntu.png)

upgarde ubuntu

`sudo apt upgrade`

![upgarding ubuntu](./images/backend-configuration/upgrading-ubuntu-step1.png) 

![upgrading ubuntu](./images/backend-configuration/upgrading-ubuntu-step2.png)

![upgrading ubuntu](./images/backend-configuration/upgrading-ubuntu-step3.png)

get the location of Node.js software from Ubuntu repositories.

`curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -`

Install node.js with the command below

`sudo apt-get install -y nodejs`

![installing node.js](./images/backend-configuration/installing-node.js-step1.png)

![installing node.js](./images/backend-configuration/installing-node.js-step2.png)

![installing node.js](./images/backend-configuration/installing-node.js-step3.png)

![installing node.js](./images/backend-configuration/installing-node.js-step4.png)

verify that node installation

`node -v`

![verifying node installation](./images/backend-configuration/vrifying-node-installation-1.png)

`npm -v`

![verifying node installation](./images/backend-configuration/verifying-node-installation-2.png)

create a new directory for Todo project

`mkdir Todo`

![verifying creation of Todo directory](./images/backend-configuration/Todo-directory-creation.png)

change current directory to newly created one

`cd Todo`

![changing to Todo directory](./images/backend-configuration/changing-to-Todo-directory.png)

`npm init`

![initialising project](./images/backend-configuration/initialising-project.png)

confirm that package.json file has been created

`ls`

![confirmin that package.json file has been created](./images/backend-configuration/confirming-creation-of-package.json-file.png)

### INSTALL EXPRESS.JS

`npm install express.js`

![installing express.js](./images/installing-express.js/installing-express.js.png)

create a file named index.js

`touch index.js`

install dotenv module

`npm install dotenv`

![installing dotenv module](./images/installing-express.js/installin-dotenv-module.png)

open index.js file and paste code

`vim index.js`

![pasting code in vim](./images/installing-express.js/pasting-code-in-vim.png)

start server with command below

`node index.js`

![starting server with command node index.js](./images/installing-express.js/starting-server.png)

open custon TCP port 5000

![opening cutom TCP port 5000](./images/installing-express.js/oprning-custom-TCP-port-5000.png)

[acccessing server IP wit browser](http://3.75.172.48:5000/)


![acccessing server IP wit browser](./images/installing-express.js/accessing-IP-with-browser-port5000.png)

routes

For each task, we need to create routes that will define various endpoints that the To-do app will depend on. So let us create a folder routes

`mkdir routes`

`cd routes`

create a file in routes directory named api.js

`touch api.js`

open file with vim

`vim api.js`

paste code in api.js with vim

![pasting code in api.js](./images/installing-express.js/api.js-code.png)

MODELS

Since the app is going to make use of Mongodb which is a NoSQL database, we need to create a model.

A model is at the heart of JavaScript based applications, and it is what makes it interactive.

We will also use models to define the database schema . This is important so that we will be able to define the fields stored in each Mongodb document.

In essence, the Schema is a blueprint of how the database will be constructed, including other data fields that may not be required to be stored in the database. These are known as virtual properties

To create a Schema and a model, install mongoose which is a Node.js package that makes working with mongodb easier.

change directory back to Todo folder and install mongoose

`npm install mongoose`

![installing mongoose](./images/models/installing-mongoose.png)

create a new folder named models, change directory to models and then create a file named todo.js inside the models directory

`mkdir models && cd models && touch todo.js`

`vim todo.js

paste code

![todo.js code](./images/models/todo.js-code.png)

open routes directory

`vim api.js`

paste code

[changing code in api.js](./images/models/changing-code-in-api.js.png)

MONGODB DATABASE

Open an mlab mongoDB account and choose AWS as cloud provider. Then choose a region near you.

Allow access to mongoDB database from anywhere.

![alowing access to MongoDB databse from anywhere](./images/MongoDB-database/allow-IP-address-from-anywhere.png)

Create a MongoDB database and collection inside mLab

![creating database and collections](./images/MongoDB-database/creating-database-and-collecctions.png)

change directory to Todo

`cd Todo`

`touch .env`

`vi .env`

add connection string below after updating <username>, <password>, <network-address> and <database> according to your setup

connection string: DB = 'mongodb+srv://<username>:<password>@<network-address>/<dbname>?retryWrites=true&w=majority'

see updated connection string below

DB =  mongodb+srv://iyereogholoh:Sy8leZAkgWJutGPB@cluster0.y38fy8p.mongodb.net/IyereDB?retryWrites=true&w=majority

![adding connection string](./images/MongoDB-database/connection-string.png)

update the index.js to reflect the use of .env so that Node.js can connect to the database

`vim index.js`

delete index.js file

![deleting the index.js file](./images/MongoDB-database/deleting-index.js-file.png)

`i`

paste new code

![pasting new code](./images/MongoDB-database/pasting-new-code.png)

start server

`node.js`


















