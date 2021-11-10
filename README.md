# Build your AI Chatbot with Zero Coding

In this workshop, we are going to create a  customer service Assistant for a bank. We are looking to automate some of the top questions that are reaching our agents via support chat on our site,in this scenario - people trying to transfer money to friends or family.

We will Start by redirecting people contextually into the bank's application if they have a transfer to make under $1000

## Prerequisites
- [IBM Cloud Account](http://ibm.biz/nocodebot)
- [Twilio Account](www.twilio.com/referral/V69RV9)


## Step 1: Sign-up/Login to IBM Cloud

1.1- If you are an existing user, click on this link to Login: http://ibm.biz/nocodebot

And if you are not, don't worry! We have got you covered! There are 3 steps to create your account on IBM Cloud: 

1.2- Put your email and password. 

1.3- You get a verification link with the registered email to verify your account. 

1.4- Fill the personal information fields. 

** Please make sure you select the country you are in when asked at any step of the registration process.

![image](https://user-images.githubusercontent.com/16270682/140926329-d798e427-5b56-4b6c-bfe7-aacf4543b24c.png)

## Step 2: Create an instance of Watson Assistance service

2.1 - Fron Dashboard search for Watson Assistant service in catalog 

<img width="585" alt="1" src="https://user-images.githubusercontent.com/16270682/140980671-23b74739-acd5-4a1d-9ed5-fb164d05f0bf.PNG">


2.2 - Check the terms box and click on create. This will take you to a new window

<img width="825" alt="2" src="https://user-images.githubusercontent.com/16270682/140980692-2de653ce-f4ea-4bc2-89c6-a179d6a7eb8b.PNG">


2.3 - Click on Launch Watson Assistant to start building your chatbot

<img width="710" alt="3" src="https://user-images.githubusercontent.com/16270682/140980716-fe3b93a3-98b1-4128-b6c6-a4f236beb33c.PNG">


2.4 - Go to top right, select manage > Switch to new experience, it will prompt a confirmation message, click on switch.

<img width="957" alt="4" src="https://user-images.githubusercontent.com/16270682/140980993-13e3a96b-29f1-4e8d-9e4e-50694575c48f.PNG">


## Step 3: Create your first assistant

3.1- Name your assistant and click on create 
<img width="718" alt="6" src="https://user-images.githubusercontent.com/16270682/140990991-b532b434-4c16-4f07-91b7-7d52a1052f51.PNG">


3.2 - From the home window, select your first action, this will take you to a new window.
<img width="521" alt="7" src="https://user-images.githubusercontent.com/16270682/140990999-45272753-e681-4bf4-ac46-f9ce886457ab.PNG">


## Step 4: Create your First action

4.1 - click on  create a new action


<img width="611" alt="8" src="https://user-images.githubusercontent.com/16270682/141001953-15ebda6a-ed8f-4f9d-8819-667cd1ed9d24.PNG">


4.2 - add "I want to transfer $100 to my friend" and click save

<img width="439" alt="8-1" src="https://user-images.githubusercontent.com/16270682/141002029-eaeb7f69-002d-49e4-9ea8-02d657a91836.PNG">


#### We are going to setup 3 steps for our action


4.3 - change the title of the action in the top left to something more consumable - "Transfer funds"

4.6 - Step 1: In our first step, enter **"How much would you like to transfer?"** and Under options, we can define the type of response we anticipate from the user. select **currency** and click on next step

<img width="687" alt="8-2" src="https://user-images.githubusercontent.com/16270682/141002064-80f377c8-ff34-4d31-b6fb-d78342d82a0e.PNG">


4.7 - Step 2: In our second step, enter **"When do you want to make this transfer?"** select **date** 

***Note that the system can detect dates in plain language, not just formatted (e.g. tomorrow, two weeks from now, etc...)***

<img width="690" alt="10" src="https://user-images.githubusercontent.com/16270682/141002082-8c9cb0fc-7ac4-402b-8dbc-5284bfce3a04.PNG">



4.7 - Step 3: In our third step, add a simple confirmation message to make sure we've got everything right. add "Just confirming, you want to transfer $ "$step1" on "$step2?"

Notice how we can use the $ sign to call upon pieces of information the user has already provided in an earlier step - these are called variables

<img width="718" alt="11" src="https://user-images.githubusercontent.com/16270682/141002097-be91b270-179d-45ea-91b2-6e2e5d55be56.PNG">

