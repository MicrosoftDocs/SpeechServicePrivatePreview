# Organization Speech Model (Private Preview) - Draft - Please Ignore

Speech transcription is becoming a very demanding functionality for both consumer users and enterprise users. The use cases range from intelligence agent, intelligent meeting, connected car, call center transcription, dictation, and video indexing. The key success factor in industry is whether the application can provide high speech recognition accuracy, where the technical challenge is how to adapt the model to your enterprises and customers. This in turn depends on how much high-quality data is used to train the model and optimize the model toward the vocabulary of your enterprise and your scenarios.   
 
Now we offer Organization Speech Model on Azure through Speech Cognitive Service for 3rd party enterprise customers. With this service, you will be able to leverage your O365 assets to generate Organization Speech Model dedicated for your enterprise within compliance boundary in just a few steps. 

Note that Organization Speech Model is now in private preview with limited slots available through private invitations. Before we enroll you in the early-adopter program, please take a few minutes to let us know more about you and your project. By submitting this form, you acknowledge that the information you provide via this form may be used for market research and your application does not guarantee admission. You will be informed if your access is granted.

Thank you for your interest in Microsoft Speech to Text services. 

## How to Onboard after Access is Granted
![OnboardingFlow](https://github.com/MicrosoftDocs/SpeechService/blob/master/quickstart/organization-speech-model/flow.png)

### Offline Enrollment
Tenant Admin go to Microsoft 365 Admin Center and turn on “Azure Speech Service” toggle. 

* Log in Microsoft 365 Admin Center https://admin.microsoft.com .
* Click on "Settings" and "Services & add-ins" on the left panel
* Search for “Azure Speech Service" and click on the link
* Turn ON the toggle and click on "Save" button
* To turn off tenant model, turn off the toggle and click on “Save” button.

### Offline Onboarding
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
  
* Call speech service based on Sample Code with AAD Auth enabled. 

## FAQ

* Q: When should I use Organizational Speech Model?
* A: If your enterprise’s jargon are available in Office 365 data (email, documents), and you want to improve speech recognition accuracy on these important terms, we recommend to opt in Organizational Speech Model.

* Q: Which Office 365 data is being used? 
* A: The service is currently trained with your company’s public communication emails. Later it will expand to include all the knowledge in your organization’s Office graph. The generated Organizational Speech Model is dedicated to only serve your enterprise with regular updates. 

* Q: Is the model generation an eyes-off process? 
* A: Yes, the model generation is an eyes-off process. It trains languages models for your organization in an eyes-off, privacy compliant environment. 

* Q: What’s the difference of Organizational Speech Model and Custom Speech Model?
* A: Organizational Speech Model is based on O365 data with automatic regular updates, while custom model is based on user manually provided data. They will compensate each other to optimize speech service in a more efficient way.

* Q: How can I measure the performance of Organizational Speech Model? 
* A: The model performance is proven positive based on internal experiment.  We will do offline measurement based on customer-provided test data before self-serve testing is enabled.
