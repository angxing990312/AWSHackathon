# AWSHackathon
![image](https://user-images.githubusercontent.com/68961012/88884705-c06d2980-d269-11ea-9623-250678ee2120.png)

Team MADD AWS Hackathon Solutions:
3 Prong approach to ACRA's Problem statement. 

> Automated Decesion Engine (RPA) 

> SinglePortalSubmission (Chatbot)

> AI-Analytic-Dashboard 

# Introduction of solutions
## Single Portal Submission (ChatBot)

**Preview** 

![image](https://user-images.githubusercontent.com/68961012/88885384-024a9f80-d26b-11ea-9375-9ac527b5c120.png)
![image](https://user-images.githubusercontent.com/68961012/88885398-08d91700-d26b-11ea-9e9e-5213310392f5.png)

**Benefits**
 
 - Single Channel Submission(To be submitted via Telegram Chatbot) 
 
 - Conversational Chatbot to communicate and answer users' enquiries. (Performed by Dialogflow)
 
 - Users can get application status updates from chatbot 
 
 - Integrated with Amazon S3 Bucket
 
 - Convenient and adoption is easy 
 
## Automated Decision Engine (RPA)

**Preview**

![image](https://user-images.githubusercontent.com/68961012/88885999-2f4b8200-d26c-11ea-9050-5de619429d4f.png)

**Benefits** 

- RPA helps to resolve reptitive and manual task

- Business rules can be set to automate straightforward cases

- Response time to customer can be speed up 

## AI Analytics Dashboard (Amazon QuickSight)

**Preview** 

![image](https://user-images.githubusercontent.com/68961012/88886266-aa149d00-d26c-11ea-9c24-539ed88ce23c.png)

**Benefits** 

- Integrates all information from different systems into one dashboard

- Integrated with Amazon Quicksight

- Tracks all the information at once and visualize user’s past performance

- Actionable insights can be provided for AOs/POs

# Demostration of Prototype

## 1. User part (Single Portal Submission (ChatBot))

First, the user will need to go to our chatbot. Click the START button to start conversation with the Chatbot. 

![image](https://user-images.githubusercontent.com/68961012/88904378-97f42800-d287-11ea-8a1b-e41373129059.png)

Then the user will need to enter their name and email, after entering, they will be given 2 choices. Submit a claim or Q&A.

![image](https://user-images.githubusercontent.com/68961012/88904874-37b1b600-d288-11ea-93bd-9bc0bac3acb3.png)

For the purpose of demonstration, I will choose "Submit a claim". After choosing "Submit a claim", Chatbot will prompt the user with notification and a "Submit Appeal" button to redirect them to the website where they will submit their appeal. 

![image](https://user-images.githubusercontent.com/68961012/88905612-084f7900-d289-11ea-91f9-faf3f7220b79.png)
![image](https://user-images.githubusercontent.com/68961012/88905946-7300b480-d289-11ea-8ee6-c3083058520c.png)

When the user have entered the website, they will need to click "SUBMIT APPEAL" to submit their appeal. 

![image](https://user-images.githubusercontent.com/68961012/88906275-d559b500-d289-11ea-93c8-7db3acc34602.png)

## 2. Software part (Automated Decision Engine (RPA))

Once the appeal case is submitted via the website, the ACRA Singtel Portal Submission will receive the case. Automated Decesion Engine(RPA) will be used to analyze the appeal case. If the case is acceptable, it will be sent to BizFile+ and stored in AWS S3 Bucket for further verification. Once verification of the case is done, Bizfile+ will send the result of appeal case to ACRA Single Portal Submission, then reply to the customer on result via TelegramChatBot. 
Below are a picture to demonstrate the whole process:

![image](https://user-images.githubusercontent.com/68961012/88919510-c977ee00-d29d-11ea-8cae-d2a7ff397156.png)

Meanwhile, another feature of our prototype is AI Analytics Dashboard (Amazon QuickSight). The purpose of this dashboard is to give the officer a quick glance on the business data of the applicant to speed up their decision process. Business data like: Annual Income of past years, 
