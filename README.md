# AppDirectCodingChallenge
Coding Challenge of AppDirect

The Application is hosted on AWS and can be found at below url

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/

Alternate way to run the application is as below 


#Instalation

The Project is created in Eclipse using Maven Build tool.

Steps  :

1) git clone https://github.com/AshishShivrajPoste/AshishPosteAppDirectCodeChallenge.git

2) mvn clean package
  Note : please change the consumerKey and consumerSecret in config.properties file under /src/main/resource before packaginf the application
3) Deploy the war generated into tomcat server.

  copy the .war generated in step 2 to tomcat webapp folder

4) start tomcat

I am using ngrok for creating the tunnel.

# Configuration

Please change the consumerKey and consumerSecret in config.properties file under /src/main/resource.



# AppDirect Event Notification URL configured

AWS hosted Application has below urls

Subscription Create Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/subscription/create?url={eventUrl}

Subscription Change Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/subscription/change?url={eventUrl}

Subscription Cancel Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/subscription/cancel?url={eventUrl}

Subscription Status Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/subscription/status?url={eventUrl}

User Assignment Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/user/assign?url={eventUrl}

User Unassignment Notification URL

http://myfirstelasticbeans-env12345.us-east-1.elasticbeanstalk.com/webapi/user/unassign?url={eventUrl}



You can change the below url if you are using local deployment on tomcat along with ngrok tunneling.

Subscription Create Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/subscription/create?url={eventUrl}

Subscription Change Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/subscription/change?url={eventUrl}

Subscription Cancel Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/subscription/cancel?url={eventUrl}

Subscription Status Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/subscription/status?url={eventUrl}

User Assignment Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/user/assign?url={eventUrl}

User Unassignment Notification URL

http://690c679c.ngrok.io/codechallenge/webapi/user/unassign?url={eventUrl}

