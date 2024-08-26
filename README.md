# OracleFusionSqlEditor

Run SQL queries on Oracle Fusion/Saas DB with this simple VBS page/app-ui

# Features
-  Built using VBS and deployed in Fusion system
-  No seperate installation required
-  Accessible like like any other fusion applciaiton page
-  No seperate authentication required

#  Limitations
-  Only 1000 rows and 1000 columns can be fetched
-  Query time out of 5 mins.

#  Access Requirements
-  Roles required to create and execute BI publihser reports

# Installaton (Only at instance level): --> Postman can also be used
-  Download the VX file 
-  Execute below curl
```
curl -v --noproxy '*' -X POST -L -H Content-Type: application/octet-stream -H 'X-OAM-AUTHN-HINT: 0' -u USERNAME:PASSWORD --data-binary @EXTENSION_NAME.vx http://INSTANCE_URL:PORT/fscmRestApi/vx/v2/extensions
```
-  After installtion execute below command and find for 'SqlAppExtn', if found the installation is successful
```
curl -v --noproxy '*' 'X-OAM-AUTHN-HINT: 0' -u USERNAME:PASSWORD http://INSTANCE_URL:PORT/fscmRestApi/vx/v2/extensions/
```

# Accessing the page
-  Post successful installation, open below url and login (if prompted)
```` https://INSTANCE_URL/fscmUI/redwood/SqlEditor ````

# Preview
-  Editor Layout
![image](https://github.com/user-attachments/assets/d85a28e0-ccc3-42b6-9ff5-11cbcd54adef)

-  Connectivity Layout
![image](https://github.com/user-attachments/assets/e5632ca9-9922-45be-8273-0ff8c851db05)

