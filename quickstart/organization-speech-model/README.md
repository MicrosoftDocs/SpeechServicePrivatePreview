# Organization Speech Model (Private Preview)

Speech transcription is becoming a very demanding functionality for both consumer users and enterprise users. The use cases range from intelligence agent, intelligent meeting, connected car, call center transcription, dictation, and video indexing. The key success factor in industry is whether the application can provide high speech recognition accuracy, where the technical challenge is how to adapt the model to your enterprises and customers. This in turn depends on how much high-quality data is used to train the model and optimize the model toward the vocabulary of your enterprise and your scenarios.   
 
Now we offer Organization Speech Model on Azure through Speech Cognitive Service for 3rd party enterprise customers. With this service, you will be able to leverage your O365 assets to generate Organization Speech Model dedicated for your enterprise within compliance boundary in just a few steps. 

Please note that this feature is now in Private Preview with limited slots. Thank you for your interest in Microsoft Speech to Text services. 

# How to Onboard
![OnboardingFlow](https://github.com/MicrosoftDocs/SpeechService/blob/master/quickstart/organization-speech-model/flow.png)

## Offline Enrollment
Tenant Admin go to Microsoft 365 Admin Center and turn on “Azure Speech Service” toggle. 

* Log in Microsoft 365 Admin Center https://admin.microsoft.com .
* Click on "Settings" and "Services & add-ins" on the left panel
* Search for “Azure Speech Service" and click on the link
* Turn ON the toggle and click on "Save" button
* To turn off tenant model, turn off the toggle and click on “Save” button.

## Offline Onboarding
Application developers follow the instructions to install the Speech SDK NuGet package and add AAD Authentication code

* Register your application in Azure to get client ID.
  * Log in https://ms.portal.azure.com/ using an account under your tenant. 
  * Click on "Azure Active Directory" and "App registrations".
  * Click on "+New application registration" to register your application and get "Application ID".
  * Refer to documentation for more details.
  
  ![Alt Text](https://github.com/MicrosoftDocs/SpeechService/blob/master/quickstart/organization-speech-model/ClientId.png)

* Get client key.
  * Click on the registered application name.
  * Click on "Settings" --> "Keys".
  * Create key and click on "Save" button.
  * Copy the key "value" before leaving the page.  The value will be hidden next time.  
   
  ![Alt Text](https://github.com/MicrosoftDocs/SpeechService/blob/master/quickstart/organization-speech-model/Key.png)
  
* Call speech service with Sample Code with AAD Auth. 


