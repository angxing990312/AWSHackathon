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
- Website (Submission purpose)

# Installation & Set-Up

- Install Dialogflow (URL: https://cloud.google.com/dialogflow/docs)
- Installed Telegram (URL: https://desktop.telegram.org/)
- Installed UIpath (URL: https://www.uipath.com/fr/start-trial)
- Installed Visual Studio (URL: https://visualstudio.microsoft.com/downloads/)

# Solution

## Single Portal Submission(ChatBot)

For Single Portal Submission(SPS), An agent will be created in the DialogFlow Console, and various intents will be created according to the required context. Within the created intent, training phases should be inserted, to train the dialog Flow agent in order to capture user's responses. We can also set this response to a binary Click-button option. Follwing the selection of option, a Prompt for submission will be created, and once the user clicks on the button, it will direct them to a web server which is directly connected to the database used for processing these appeal cases. System entities(Object identifier) should be created to validate the User's personal details for the appeal submission.

Lastly, the dialog Flow agent will be linked to the telegram platform ChatBot. (Other chatbots can also be link. e.g Facebook messenger, twitter and Viber)

Step 1: Create a Telegram Bot through @Botfather. (Insert image)
Step 2: Copy the generated token number.
Step 3: Paste the Token number into the dialog Flow Agent through the "integrations" tab.(Insert image)
Step 4: Enable Fulfillment (Connecting the WebHook)


## Automated Decision Engine(RPA)

When the new case is being submitted, it would trigger UIPath to analyse the new cases. It would help to automate straightforward cases and eliminate the need for the officer to route the cases manually. A new record will be created for the acceptable cases(Details fully filled up, with supporting documents). Then, a template that contain relevant information will be created and all these document will be routed to officer for review. Not acceptable cases will be reject and a email will be sent to inform customer. 

## AI Analytic Dashboard(Amazon Quicksight) 

For the AI Analytic Dashboard, it is used by the ACRA officer to assist them in making judgement on appeal cases. The implementation of Amazon Quicksight could help to integrate relevant dataset from different places, E.g. Acra database, Amazon S3 Bucket etc to generate a meaningful dashboard to provide a glanace view of applicant past performance. Different report can be created on top of these information to cater for different business need. Data can be visualize and generated as chart by integrating different data together. 

Charts for example: 

- Average Company Credit Score
- Overview of past Approved and rejected cases
- Past Year Annual Income  by Case Number
- Overview of past Appeal cases processing time and Status 

From the above charts, it helps officers to make a final judgement on should they approve the case or reject it. 

