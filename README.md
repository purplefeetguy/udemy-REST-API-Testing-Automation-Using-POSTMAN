# udemy-REST-API-Testing-Automation-Using-POSTMAN

## StudentApp needs JAVA 8
Make sure you install JAVA 8 and then set JAVA_HOME to that install dir.
### On Windows 10
echo $Env:JAVA_HOME C:\Program Files\Java\jdk1.8.0_221


Once JAVA 8 is installed and JAVA_HOME set, navigate to where you have extracted StudentApp.zip and run:

java -jar rest.jar

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v1.4.2.RELEASE)

Validate the app is running by opening a browser and navigating to:

http://localhost:8080/student/list

[{"id":1,"firstName":"Vernon","lastName":"Harper","email":"egestas.rhoncus.Proin@massaQuisqueporttitor.org","programme":"Financial Analysis","courses":["Accounting","Statistics"]},{"id":2,"firstName":"Murphy","lastName":"Holmes","email":"faucibus.orci.luctus@Duisac.net","programme":"Financial Analysis","courses":["Accounting","Statistics"]},{"id":3,"firstName":"Reece","lastName":"Jason","email":"tincidunt.dui@ultricessit.co.uk","programme":"Computer Science","courses":["Calculus","Algorithms","Software Development","Ethics"]},


There will be much many more entries...


If you have a port conflict (something already on port 8080) start against a port not in use.

java -jar rest.jar --server.port=8085

Update your URL accordingly:

http://localhost/8085/student/list

[{"id":1,"firstName":"Vernon","lastName":"Harper","email":"egestas.rhoncus.Proin@massaQuisqueporttitor.org","programme":"Financial Analysis","courses":["Accounting","Statistics"]},{"id":2,"firstName":"Murphy","lastName":"Holmes","email":"faucibus.orci.luctus@Duisac.net","programme":"Financial Analysis","courses":["Accounting","Statistics"]},{"id":3,"firstName":"Reece","lastName":"Jason","email":"tincidunt.dui@ultricessit.co.uk","programme":"Computer Science","courses":["Calculus","Algorithms","Software Development","Ethics"]},

Users who have JAVA 9 installed can start the app using the below command
java -jar --add-modules java.xml.bind rest.jar