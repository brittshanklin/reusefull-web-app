# Re.Use.Full
## [System Context Diagram](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Reusefull.SystemContextDiagram#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1QKiP_kJ8_0XHahV5Tgk3Iaksb6THSV5Y%26export%3Ddownload)
## [Application Context Diagram](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Reusefull.AppContextDiagram#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1CONXQebsTXZhY1Vvfp6QXttBu_KPy6aw%26export%3Ddownload)
# Docker
The app is deployed in a docker container.  There is a file naed reusefull.env in home\ec2-user folder.  The ec2-user folder has a subfolder named .docker.

# To run this app locally for testing:
* Copy this repo locally
* Set some environment variables. The only way I have figured out so far to do this on Windows is to edit the Windows Environment variables one at a time.  We have a test database you can connect to.  Many of the parm values don’t matter but are needed for the app to start.  Add the following “System variables” in your Environment variables.  The values for the variables will be provided to you as needed.
  * AUTH0_CLIENT_ID	reusefull
  * AUTH0_CLIENT_SECRET	reusefull
  * AUTH0_LOGOUT_URL	reusefull
  * AUTH0_REDIRECT_URL	reusefull
  * DGRAPH_TOKEN		reusefull
  * HERE_TOKEN		reusefull
  * MYSQL_DB			xxx
  * MYSQL_HOST		xxx.xxx.xxx
  * MYSQL_PASS		xxx
  * MYSQL_USER		xxx
* Open a terminal in your IDE with the code (possible Visual Studio Code)
  * Go run .
  * Yes, the above is the word “go” followed by a space, then “run” then a space then a period.  The period tells go to compile and run all the code.
  * You should get a message in your terminal that says “Successfully started”
  * Then you can open a browser to http://127.0.0.1 and you should see the site.  Click on the Donors tab and select Donate - this will cause a database connection attempt.
 
  * In DBeaver, you may also need to change Driver Properties (allowPublicKeyRetrieval to true and useSSL=false ) 
