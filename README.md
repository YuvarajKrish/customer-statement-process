# customer-statement-process

Demo for Rebo Bank Statement processor on Customer Transaction



* Only pom.xml and Source file are there , so please check out the jars using maven.
* Application run in 9001 Port.
* Once run application , post rest-service with accepting multipart form data will run
* 


Import & Run : 
* Import the project in IJ or Other ID
* Application build on Java8 and Junit5 ( set the runner as junit5)


Business Logic:
* Strategic Design patter were used to Process the files ( Two file processors) to read the data file and Scheduler been configured to trigger the process ( once - if 
	required we can configure with crons) , Invalid records details are printed in console.


 
How to Run:

We can create runnable jar ( by mvn clean install ) or importing in IDE and running the spring boot class

Application will run in 9001 Port
Rest Service Url will be : http://localhost:9001/rabo/customer/statement/processor 
Method: Post
Body : 	set content type as : multipart/form-data
		field name as : Records
		choose file as : File to test 


When running application as jar - will create log & multipart file (request file ) in same the folder for reference.


How to Test Junit:

- Need to run as Junit5
- Before run the test case , recommand to  run & test once the application are working as expected in IDE will good. 

