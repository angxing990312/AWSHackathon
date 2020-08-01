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

- Install Dialogflow (URL: https://cloud.google.com/dialogflow/docs)
- Installed Telegram (URL: https://desktop.telegram.org/)
- Installed UIpath (URL: https://www.uipath.com/fr/start-trial)

# solution

## Single Portal Submission(ChatBot)

For the SPS, user must link Dialogflow to Telegram(Setting up of Chatbot).  


## Automated Decision Engine(RPA)

For the ADE, UIpath will receive appeal cases from SPS. Then UIpath will filter all the cases. Those acceptable cases(Details fully filled up, with supporting documents) will be routed to AWS S3 Bucket and BizFile+ for further verification. Not acceptable cases will be sent back to SPS. SPS will then inform the customer on the information they need to fill up in the appeal form. 

## AI Analytic Dashboard(Amazon Quicksight) 

For the AIAD, it is used by the ACRA officer to assist them in making judgement on appeal cases. The officer can just simply upload the business data provided by customer onto QuickSight, generate charts using the data. 

Charts for example: 

- Average Company Credit Score
- Overview of past Approved and rejected cases
- Past Year Annual Income  by Case Number
- Overview of past Appeal cases processing time and Status 

From the above charts, it helps officers to make a final judgement on should they approve the case or reject it. 
