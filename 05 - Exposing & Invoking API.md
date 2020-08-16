4. Exposing and invoking the API
4.1. API Management Login
Open the Red Hat 3scale API Management Platform Login screen.

Select the Red Hat Single Sign On option. This triggers an OAuth Flow and redirects you back to the Red Hat 3scale API Management Platform Dashboard.

Dismiss the How does 3Scale work? option which is displayed the first time you log in to Red Hat 3scale API Management Platform. The main Dashboard is displayed.

Check your workCheck your work
Can you see the Red Hat 3scale API Management Platform Dashboard and navigate the main menu?

Check your work

Yes

No
4.2. Adding the App Endpoint to Red Hat 3scale
From the APIs section of the Dashboard, select the New Product item.

Select the Import from OpenShift option. If this option is not enabled, click Authenticate to enable this option

Choose the fuse option from the Namespace list.

Choose i-greeting-api from the Name list.

Click Create Product.

This process can take a few minutes.

Edit the API:

Choose Product: i-greeting-api from the top navigation menu to view the Overview page.

Select the Settings item in the Integration dropdown menu.

In the Staging Public Base URL, enter:

https://wt3-evals02-3scale.apps.dfw-7226.example.opentlc.com

Click Update Product at the bottom of the page.

Create a mapping rule for the /greeting endpoint.

Select the Mapping Rules item in the Integration dropdown menu.

Click Add Mapping Rule

Select POST in the Verb field

Enter /greeting in the Pattern field

Click Create Mapping Rule at the bottom of the page

Check your workCheck your work
Is the new mapping rule visible from the Mapping Rules screen?

Check your work

Yes

No
4.3. Configuring your API
Create a new Application Plan:

Select Applications > Application Plans from the side navigation.

Select Create Application Plan.

Enter the following for Name and System name:

low-code

Leave the other fields with their default values.

Select Create Application Plan. You will be redirected to the Application Plans screen.

Click Publish, beside your plan list item, to publish the Plan.

Create a new Application for the Developer Group, assigned to the Plan:

Select Audience from the top navigation menu.

Select the Developer Account to open the Account Summary page.

Select the (num) Application item from the breadcrumb to view Applications.

Select the Create Application button in the top right.

Select the low-code Plan in the Application plan menu.

Enter the following for Name and Description:

low-code-app

Select Create Application.

Set a custom User Key for the application:

On the low-code application screen you were redirected to, scroll to the API Credentials section.

Click the green pencil icon beside the User Key

In the Set Custom User Key modal dialog, enter:

test

Select Set Custom Key.

Check your workCheck your work
Review the settings in 3scale. Do they match the settings outlined in this task?

Check your work

Yes

No
4.4. Staging your API
Click the Configuration menu item in the Integration dropdown menu from the side navigation.

In the APIcast Configuration section, click the Promote to Staging button

Check your workCheck your work
Is a new version of the API visible in the Environments section of the page?

Check your work

Yes

No
4.5. Invoking the API
Use an HTTP client to invoke the route, for example:

curl -d '{"name":"John"}' -H "Content-Type: application/json" -X POST "https://wt3-evals02-3scale.apps.dfw-7226.example.opentlc.com/greeting?user_key=test"

Check your workCheck your work
Did the message "Hello from John appear in your Slack channel?

Check your work

Yes

No

____
## Congratulations you have completed this lab!
____

<p align="center">
  <a href="/04%20-%20Implement%20Operations.MD">Previous Exercise</a> &nbsp;|
  &nbsp;<a href="/README.md">Table of Contents</a> &nbsp;
</p>

[1]: https://tutorial-web-app-webapp.apps.dfw-7226.example.opentlc.com/
[2]: https://fuse-2dd27faf-dfda-11ea-a6a0-0a580a010007.apps.dfw-7226.example.opentlc.com/
