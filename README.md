# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.


![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/d1fbe485-3197-4600-87c2-16852b21049d)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.


![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/98bb65f6-8307-44a9-94e5-03583a171713)

 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.



![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/17abcc70-0a75-4e86-89de-3884299ed5c8)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/c54e927d-f230-4ad7-8327-123484ed33d3)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.



![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/cbe48cb0-751d-47b5-8a06-1b81b562a13b)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 
Step 4: Carefully select your RESTful resource (web service) and click OK.
 



![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/244a3f8b-316d-435b-ada7-e4b2e348a8fe)




Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.



![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/3f9590d4-14a8-428f-a896-3b677d1a1a5b)



Step 6: An editing tab will open. Alter getHtml() method with the following.



 ![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/0db16713-7514-4ef5-b59e-8707e95de566)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/0b053afb-0a83-4801-96f9-83a979c50d6e)



Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 

![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/509ceb67-b83d-4bd9-a11f-e6e36b7f3bac)




Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.


![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/12c08f6d-26b1-472e-9c1d-151b24b997a5)




Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
![image](https://github.com/nanditha121/Ex-04_RESTful_Web_Services/assets/142209508/26e5a449-4d97-48a7-a733-f9f169b08960)


  

Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
