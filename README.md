# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
**Step 1**: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

**Step 2**: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/a45e9a94-15c0-4f25-8af8-0f9290928969)


**Step 3**: A new window will appear. Select “Simple Root Resource” and click Next.
 
![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/8c46f626-a53a-4148-9f8d-ae227b1555e9)


**Step 4**: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/ef5c6ada-0f70-4929-a730-1feb3c09a490)


**Step 5**: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

**Step 6**: Alter getHtml() method as shown below.

**Step 7**: Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/5d8e1073-f6f0-4928-a147-bbef9be2bf06)

 


**Step 8**: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



### Client-Side:


**Step 1**: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

**Step 2**: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/20d97d6f-d836-44f2-93a4-6e6aa3b170f6)


**Step 3**: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

**Step 4**: Carefully select your RESTful resource (web service) and click OK.
 
![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/823edd4e-02ac-470d-a01c-e8dedcf280f7)
 

**Step 5**: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/03cc9db3-efac-4eda-b799-b71568ff9b6e)


**Step 6**: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/ea9a5ae2-b4dc-452b-ab30-2d950667f943)


**Step 7**: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/a16cae89-4de4-4826-9c67-3c281908a52d)


**Step 8**: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/d3ee7aab-f952-494a-a170-39cfa1e55379)


**Step 9**: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

**Step 10**: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/0f4a44df-ab7c-42b0-a16b-03bc7edbedfb)


**Step 11**: Save the project and build it.

**Step 12**: Run the JSP file and you should see the output in a new browser window.


 
![image](https://github.com/Mena-Rossini/Ex-04_RESTful_Web_Services/assets/102855266/f495b738-83a4-452b-824e-9e7a81515133)





### Client-Side Remote Invocation:

**Step 1**: Follow steps 1-5 as in Section 2.2

**Step 2**: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

**Step 3**: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
