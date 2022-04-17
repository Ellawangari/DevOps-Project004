# DevOps-Project004

****Project Implementation****
Technology Stack used was **MEAN**( MongoDB ExpessJS Angular Node.js)

**Step 1: Creating an AWS instance & Connecting to it using the AWS Web Console**
-![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/1.PNG)
-![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/2.PNG)
- Did a `sudo apt update` and `sudo apt upgrade`
- Added certificates `sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates`
`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -` 
![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/3.PNG)
- Installed Node js `sudo apt install -y nodejs`

**Step 2: Installing MongoDB**
> `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6`
> `echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list` 
- Install Mongo DB `sudo apt install -y mongodb`
 ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/4.PNG)
- Started the Server `sudo service mongodb start`
- Verified if the service is up and running `sudo systemctl status mongodb`
   ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/5.PNG)
- Installed Node package manager npm and installed also body parser so as to process json requests from the server
   `sudo apt install -y npm`  `sudo npm install body-parser`
    ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/6.PNG)
    
 - Created a folder called Books  `mkdir Books`   and initalize npm project  `npm init`
 - Created a server.js file and added code to it.
   ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/7.PNG)

**Step 3: Installing Express and Setting up Routes**
- installed express mongoose  `sudo npm install express mongoose` .The mongoose package installed is to enable one to create MongoDb Schemas
    ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/8.PNG)
    
 - Created an apps folder and added a routes.js file to it and added some code to it.
      ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/9.PNG)
          ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/10.PNG)
 - On the apps folder also created a models folder and added a book js file and added some code to it.
       ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/11.PNG)
          ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/12.PNG)
          
  **Step 4:Accessing the Routes with Angular**
  - On the books directory i added a folder called public and added a script.js file which i then added some code to the file.
  - Also on the same folder i created another file called index.html added code to it.
  -  Started the server by running  `node server.js`
  -  Ensured i had open tcp port 3300 and accessed my Web Book register via the browser.
      ![alt text](https://github.com/Ellawangari/DevOps-Project004/blob/main/Images/13.PNG)
      
      
   ** This Project was truly an awesome experience as I got to learn new technologies.**
**End of DevOps Project 4**
To try this project  [darey.io](https://www.darey.io) has a free trial to which you can practice this project.
    
 


