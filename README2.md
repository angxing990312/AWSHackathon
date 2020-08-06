![image](https://user-images.githubusercontent.com/68961012/88884705-c06d2980-d269-11ea-9623-250678ee2120.png)

# AWSHackcathon 
MADD Technology aims to help ACRA resolve their current pain points in waiver appeal process. 

# Content Page 
> 1. Prerequisites
> 2. Installation & Set-Up
> 3. Solution

# Prerequisites

Before you begin, ensure you have met the following requirements:

- Fully functional AWS account(QuickSight Service/S3 Bucket Database)
- Website(Submission purpose)

# Installation & Set-Up
a
- Install Dialogflow (URL: https://cloud.google.com/dialogflow/docs)
- Installed Telegram (URL: https://desktop.telegram.org/)
- Installed UIpath (URL: https://www.uipath.com/fr/start-trial)

# Solution

## Single Portal Submission(ChatBot)

For Single Portal Submission(SPS), An agent will be created in the DialogFlow Console, and various intents will be created according to the required context. Within the created intent, training phases should be inserted, to train the dialog Flow agent in order to capture user's responses. We can also set this response to a binary Click-button option. Follwing the selection of option, a Prompt for submission will be created, and once the user clicks on the button, it will direct them to a web server which is directly connected to the database used for processing these appeal cases. System entities(Object identifier) should be created to validate the User's personal details for the appeal submission.

Lastly, the dialog Flow agent will be linked to the telegram platform ChatBot. (Other chatbots can also be link. e.g Facebook messenger, twitter and Viber)

Step 1: Create a Telegram Bot through @Botfather. (Insert image)
Step 2: Copy the generated token number.
Step 3: Paste the Token number into the dialog Flow Agent through the "integrations" tab.(Insert image)
Step 4: Enable Fulfillment (Connecting the WebHook)


## Automated Decision Engine(RPA)

For the Automated Decision Engine(ADE), UIpath will receive appeal cases from SPS. Then UIpath will filter all the cases. Those acceptable cases(Details fully filled up, with supporting documents) will be routed to AWS S3 Bucket and BizFile+ for further verification. Not acceptable cases will be sent back to SPS. SPS will then inform the customer on the information they need to fill up in the appeal form. 

## AI Analytic Dashboard(Amazon Quicksight) 

For the AIAD, it is used by the ACRA officer to assist them in making judgement on appeal cases. The officer can just simply upload the business data provided by customer onto QuickSight, generate charts using the data. 

Charts for example: 

- Average Company Credit Score
- Overview of past Approved and rejected cases
- Past Year Annual Income  by Case Number
- Overview of past Appeal cases processing time and Status 

From the above charts, it helps officers to make a final judgement on should they approve the case or reject it. 

