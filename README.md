# FRT-HealthBot-FinalProject
AI Health Bot using Azure
azure-health-bot
Deployed a Azure Health bot using Azure Services. The Project intregates simple bot which is made with QnA Maker in a static website which help end users to enquire about covid-19 related information. Increase in demand for health service and enquiry about Covid19 has produce overhead for healthcare professionals and Customer service workers.Customer service, covid helpline and Hospital helpline were overwhelmed during this pandamic. Many people called helpline to enquire about covid which made created overwhelm ,which made people searching for emergency services difficult. Website for health service could include health bots which would reduce this overhead. Advantage is that In general it would make easiler for end users to search for covid norms ,book vaccine and so on. Medical chatbots would help by reducing hospital visits, reducing unnecessary treatments and procedures, and decreasing hospital admissions and readmissions as treatment compliance and knowledge about their symptoms improve. For patients, this comes with a lot of benefits: less time spent commuting to the doctor’s office less money spent on unnecessary treatments and tests easy access to the doctor at the push of a button. People can easily search for queryor book an appointment just by chatting with the bot.

Project Description Bot-Services-QnAMaker-and-Knowledgebase
![image](https://user-images.githubusercontent.com/78140862/155737125-e8765b82-5390-4765-80cd-136426c9f579.png)


Setting up the Environment QnA Maker

Create Azure resource from create resource and navigate to QnA Maker Choose Free pricing tier, select appropaite location for App Service Plan, Azure search and Also enabled App insight for Telemetry and chatlogs which will be stored here. Tasks Screenshot (o
![image](https://user-images.githubusercontent.com/78140862/157388037-4e53f826-64b6-4a3a-934a-06460eaaf734.png)

Go to view Resource and navigate to Quick start and go to QnA Portal. Add appropaite details and fill the knowledge base Screenshot (p

Tasks
![image](https://user-images.githubusercontent.com/78140862/157388690-6e0a5850-e1b7-4425-8a23-ab14d5eb7513.png)



Press Create. With Knowledge base editor we add new sets of QnA or Configure the questions. We navigate to save and train to save the changes. testKB1
![image](https://user-images.githubusercontent.com/78140862/155737369-94428b26-8844-426a-b871-43e2a174b29b.png)

Tasks We Publish the Bot by navigating to publish. To Publish we need Azure bot service. QnA portal will redirect to create Web App For Bot (Azure bot service) which will host the bot and provide tools for deployment services. We either create a new service or link a exisiting service.

Azure Bot Service

We create a azure bot service from Azure portal.


Tasks

In Azure Bot Service Under settings we go to channels copy the embeded code and secrete and replace 'YOUR_SECRET_HERE' in embed code with secret key and paste in html file.

(Code:iframe src='https://webchat.botframework.com/embed/healthbotservice-bot?s=YOUR_SECRET_HERE' style='min-width: 400px; width: 100%; min-height: 500px;'></iframe> ) Screenshot (s)

Tasks

Creating website to host Azure Bot Create an html file and the embed code with secret key Screenshot (6)
![image](https://user-images.githubusercontent.com/78140862/155737452-1a992cae-b21e-4483-b0a9-07801090dbd1.png)

Tasks Storage Account

Again we navigate to storage account from Azure portal and create storage account.

In Storage Account Under Data Management we go Static webiste enable it. we add document name to index.html referring to our website html file and Save it.

Tasks

We successfully hosted our website web

![video](https://user-images.githubusercontent.com/91495338/152352748-d9ae0c29-7e80-471c-b03a-5b1dacf79975.mp4)
Task

Summary With Azure QnA Maker, Azure QnA Maker and Azure Storage Static web hosting, we have configured a chatbot service which has capability to answer covid-19 related questions.

