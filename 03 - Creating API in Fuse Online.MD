# Creating an API Integration in Fuse Online  

## Creating an Integration with API details  

In this procedure, you create an integration with an API and include a data type. A Data Type represents a data structure that can be passed to your API and can then be used as parameters in your API definition and within the Fuse Online Integration Flow Editor to transform and map data as part of an Integration.

1. Log in to the Red Hat [Fuse Online Console][2] if you are already not. Ensure you use your username assinged to you.
```
Username: evalsXX
Password: peTG3NvNzcTK1bi
```.

2. Choose ```Connections``` link from the left navigation  menu to create a new Database connection.

![Login](images/CreateDBConnection.png)

Choose Integrations from the left navigation menu.

Click the Create Integration button to start the New Integration wizard.

Choose API Provider on the subsequent Choose a Start Connection screen.

When prompted choose Create and click Next to navigate to the API Designer.

Rename your API from "Untitled API" to:

Greeting API

Edit the Description:

My greeting API

Click Add a data type under the Data Types heading on the left of the API Designer screen.

In the Enter Basic Information section enter the following in the Name field:

Name

Enter the following JSON in the Enter JSON Example field:


{    "name": "shadowman"}

Scroll down and click Save.

Check your workCheck your work
Is </> Name listed under the Data Types on the API Designer screen?

Check your work

Yes

No
2.2. Creating a POST Resource Path
A Path represents an API endpoint/operation and the associated parameters required to invoke it.

Click Add a path under the Paths heading on the left of the API Designer screen.

In the window that appears, enter the following in the Path field:

/greeting

Click Add to confirm your entry.

Click your new /greeting endpoint under the Paths heading.

Click Add Operation under the POST icon in the Operations section on the right.

Enter the following in the Summary field:

Greet with name

Enter the following in the Operation ID field:

greetname

In the Request Body section, click Add a request body.

Choose Name as the type.

In the Responses section click Add a response.

In the window that appears choose 200 OK as the option.

Click Add.

Click No description beside the 200 OK response and enter the following in the Description field:

Greeting response

Choose String as the type. Fuse Online automatically completes the type String as String.

Click Save in the top right corner of the page to save your work. The New Integration wizard is displayed.

Click Next.

Click Publish on the New Integration wizard screen.

When prompted to Give this integration a name:

Enter the following in the Integration Name field:

Greeting Integration

Enter the following in the Description field:

my greeting api

Click Save and Publish to save your API design.

Check your workCheck your work
Is a Greeting Integration entry listed in the Fuse Online Home screen?


<p align="center">
  <a href="/README.md">Previous Exercise</a> &nbsp;|
  &nbsp;<a href="/README.md">Table of Contents</a> &nbsp;|
  &nbsp;<a href="/02%20-%20Get%20Started.MD">Next Exercise</a>
</p>

[1]: https://tutorial-web-app-webapp.apps.dfw-7226.example.opentlc.com/
[2]: https://fuse-2dd27faf-dfda-11ea-a6a0-0a580a010007.apps.dfw-7226.example.opentlc.com/