Requirments : Node.js 
Metamask
Python 
FastAPI
MySQL Database (port – 3306)

steps to set up :
1.Open a terminal.

2. Download and install Ganache.

3.Create a workspace named developement, in the truffle projects section add truffle-config.js by clicking ADD PROJECT button.

4.Download Metamask extension for the browser.

5.Now create wallet (if you don't have one), then import accounts from ganache.

6.Add network to the metamask. ( Network name - Localhost 7575, RPC URl - http://localhost:7545, Chain ID - 1337, Currency symbol - ETH)

7.Open MySQL and create database named voter_db. (DON'T USE XAMPP)

8.In the database created, create new table named voters in the given format and add some values.
    CREATE TABLE voters (
    voter_id VARCHAR(36) PRIMARY KEY NOT NULL,
    role ENUM('admin', 'user') NOT NULL,
    password VARCHAR(255) NOT NULL
    );
    Install truffle globally

9.npm install -g truffle
10.Go to the root directory of repo and install node modules
npm install
11.Install python dependencies
pip install fastapi mysql-connector-python pydantic python-dotenv uvicorn uvicorn[standard] PyJWT
