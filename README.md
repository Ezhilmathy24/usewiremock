**Guide on how to create and use wiremock for testing Rest Api`**

**Usage**: Wiremock help to test the Api developed by mocking the reponse. This enables user/ Developer to test the various scenario when the resouce to access is not readily available due to various reasons. 

**Prerequisites and bare minimum**: 
1. Docker desktop to enable running to docker which enables standalone apps to run.
2.  **docker-compose.yml** file to run the application as standalone application so the API can access the resource
2.** Request and simple reponse** to be mentioned in **mappings folder**
3. Any response that huge file format needs to placed in seperate folder **__files**

   Most common URLs required
   Url which gives you all the list of mappings ( request and reponse) created in one place.
   GET    http://localhost:8090/__admin/mappings

   RESET Url this helps to refresh and get the latest changes done in the mappings and __files folder without restarting the docker compose file.
   POST  http://localhost:8090/__admin/mappings/reset

   SHUTDOWN Url used to shutdown the wiremock docker from postman
   POST  http://localhost:8090/__admin/shutdown

   
