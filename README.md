# national-park-service-chatbot
The chatbot uses Watson Conversation, Weather Company Data, React, Nodejs, and IBM Cloud to create a chatbot about National Parks.
Chatbots and Watson: Let’s talk about national parks: course source code

The chatbot uses Watson Conversation, Weather Company Data, React, Nodejs, and IBM Cloud to create a chatbot about National Parks.

The complete course content and videos lives here

Try the live demo here

## Ask:
* which parks can you talk about
* Tell me about zion
* What animals live there
* What's the weather like
* What animals live at Denali National Park
* What's the weather like there

## Prequisities
1. Clone this repo
2. Create an IBM Cloud account

## Setup
### Conversation
* Provision an instance of Watson Conversation on IBM Cloud
* Create a new conversation workspace by importing ./resources/conversation_workspace.json into your Watson Conversation workspaces,
* Install client and server dependencies
* Create .env files in the project root
```
APP_ID=parks-conversation
PORT=3004
LOG_LEVEL=debug
SESSION_SECRET=test

WATSON_CONVERSATION_API_ROOT=https://gateway.watsonplatform.net/conversation/api
WATSON_CONVERSATION_VERSION=v1
WATSON_CONVERSATION_VERSION_DATE=2016-07-11
WATSON_CONVERSATION_USERNAME=<USERNAME>
WATSON_CONVERSATION_PASSWORD=<PASSWORD>
WATSON_CONVERSATION_WORKSPACE_ID=<WORKSPACE>
```
## Server
### Install server dependencies
```
npm install
```
## Client
### Install client dependencies
```
cd client
npm install
```
## Build / Run (Development)
* Start the server npm start
* Start the client cd client && npm start
* Navigate to http://localhost:3000
## Build / Run (Production)
```
cd client
npm run build
cd ..
npm start
```
Navigate to http://localhost:3000
## Deploy to IBM Cloud
### Prequisites:
* Install CloudFoundry Tools
* Deploy
* Follow the first 3 steps in the "Build / Run (Production)" section above, then run.
```
cf push USER_ID-nationalparks
```
Navigate to https://USER_ID-nationalparks.mybluemix.net
