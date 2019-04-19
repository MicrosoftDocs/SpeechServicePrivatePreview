# Organization Speech Model

Quickstart | Description 
------------ | -------------
[Organization Speech Service](https://opensource.microsoft.com/codeofconduct/) | For O365 enterprise customers opting in for this service, system will automatically generate a custom model leveraging the existing O365 data set to deliver high speech accuracy with minimal cost. 

![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)

# Offline Enrollment
Tenant Admin go to Microsoft 365 Admin Center and turn on “Azure Speech Service” toggle. 

* Log in Microsoft 365 Admin Center https://admin.microsoft.com .
* Click on "Settings" and "Services & add-ins" on the left panel
* Search for “Azure Speech Service" and click on the link
* Turn ON the toggle and click on "Save" button
* To turn off tenant model, turn off the toggle and click on “Save” button.

# Offline Onboarding
Application developers follow the instructions to install the Speech SDK NuGet package and add AAD Authentication code

* Register your application in Azure to get client ID and key.
  * Log in https://ms.portal.azure.com/ using an account under your tenant. 
  * Click on "Azure Active Directory" and "App registrations"
  * Click on "+New application registration" to register your application and get "Application ID"
  * Refer to documentation for more details.
* Get client key.
  * Click on the registered application name.
  * Click on "Settings" --> "Keys"
  * Create key and click on "Save" button.
  * Copy the key "value" before leaving the page.  The value will be hidden next time. 
* Call speech service using Sample Code with AAD Auth. 


