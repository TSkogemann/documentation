---
currentMenu: deeplink
---

# Deeplink

You can open the NStack website with direct access to one specific application

![App open sequence](../images/Deeplink/deeplink1.png)

The url needed looks like this

`https://nstack.io/deeplink/{appplicationId}/{masterKey}`

When an user is clicking the url, the following steps will happen:

1) Check if user is logged, else ask them to login or create an account.

**If the user creates an account that will automatically be assigned given the permission level of owner. It is very important that you do not expose the masterkey or the full link as anyone will be able to login to your application using it** 

2) Prompt user that they are about to login to the specific app

3) Check if user has access to the application, else give user access

4) Redirect to application landing page
