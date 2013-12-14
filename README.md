tomcat-automate-ant
===================

creating and deploying war in tomcat &amp; start and stop tomcat with ANT

STEP 1 :  Create a sample project with any name like WelcomeApp
              
         WelcomeApp
         |
         |-->src
         |   |
         |   |-->com.sample.TestApp
         |
         |--->war
         |    |
         |    |--->WEB-INF
         |        |
         |        |-->lib
         |        |-->web.xml
         |
         |-->index.jsp  
         |
         |-->build.xml
         |-->build.properties
         
         
STEP 2 : Change project in build.xml file
         
         <project name="WelcomeApp" basedir="." default="usage">
         
         <property name="name" value="WelcomeApp"/>
         
STEP 3 : Change tomcat home in build.properties file
          
              appserver.home = F:/Tomcat 7.0.27 [ change to tomcat installation directory ]
              
              tomcat.manager.url = http://localhost:2020/manager [ change port number ]
              
              tomcat.manager.username = tomcatuser   [ change username ]
              
              tomcat.manager.password = tomcatpassword  [ change password ]
              
              
STEP 4 : open the command prompt / terminal 
         
         Change to  C:/WelcomeApp > ant  ( press Enter )
         
         
STEP 5 : It will displays all the tasks, then choose your prefered task like,
         
         C:/WelcomeApp > ant build
                     
                       > ant deployewar
                       
                       > ant tomcat-start
                       
                       > ant list
                       
                       > ant tomcat-stop
                                       
