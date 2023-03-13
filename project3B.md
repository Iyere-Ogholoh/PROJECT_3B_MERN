#PROJECT-3B-MERN STACK IMPLEMENTATION

##BACKEND CONFIGURATION

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



