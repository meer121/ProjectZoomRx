# ProjectZoomRx

For running 2 Tomcat containers
docker pull tomcat
docker run -d --name tomcat_server_1 -p 8080:8080 tomcat
docker run -d --name tomcat_server_2 -p 8090:8090 tomcat

For creating a nginx container 
Docker build . (Builds from Dockerfile given in Github which will create an (nginx) image along with the loadbalancing configuration)
docker run -d --name nginx_server -p 80:80 nginx

Web App
To be deployed in Tomcat_server_1 and Tomcat_server_2
Note: Have pasted a single code in repository. Index.jsp in ProjectZoomRx/webapp/src/main/webapp/index.jsp to be modified as
For Tomcat_server_1
<h1> Hi Meer, This is server 1   </h1>

For Tomcat_server_2
<h1> Hi Meer, This is server 2   </h1>
