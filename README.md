# Database Backup Tool
Web-based MySQL/MongoDB/PostgreSQL database backup tool created with Node.js and React. Supports both local and cloud (Amazon S3 / Google Cloud Storage) backups.
## Requirements
The following requirements must be met in order to run this application:
- forever
``` bash
npm install -g forever
```
- nodemon (only for the development server)
``` bash
npm install -g nodemon
```
- mysql-client
``` bash
apt-get install mysql-client
```
- mongodb-org-tools
``` bash
apt-get install mongodb-org-tools
```
- postgresql-client-10
``` bash
apt-get install postgresql-client-10
```
## Installation
Use the following commands for installation:
``` bash
# install modules
npm install
# build backend
npm run build
# build frontend
npm run build-client
```
## Configuration
The following JSON configuration file is being used for initial configuration (config.json):
``` json
{
    "mongoDBUri": "",
    "secret": ""
}
```
Parameters:
- mongoDBUri: Connection string for MongoDB
- secret: Any string for express-session
## Start
Use the following command to run production server with forever:
``` bash
npm start
```
If you want to run a development server instead, then use the following command:
``` bash
npm run dev
```
