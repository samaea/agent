# Install, Build

(Below instructions were copied from https://github.com/tompaana/intermediator-bot-sample)

1. To set this up, follow these steps:

1. Make sure you have Node.js installed

1. Clone or download this repository

1. Inside index.ts, update the line below with your bot's endpoint:

   * fetch("http://YOUR_BOT_ENDPOINT/api/agent/1")

    * Example: fetch("http://mybot.azurewebsites.net/api/agent/1")

1. Inside index.ts, update the line below with your bot secret key (which you can find in your Bot Service)
    ```
    iframe.src = 'botchat?s=YOUR_DIRECTLINE_SECRET_ID';
    ```
1. Run npm install to get the npm packages

    * You only need to run this command once, unless you add other node packages to the project
    * If you encounter error TS2300, run npm install typescript@2.0.10

1. Run npm run build to build the app

    * You need to run this every time you make changes to the code before you start the application

1. Run npm run start to start the app

1. Go to http://localhost:8080 to see the Agent UI
