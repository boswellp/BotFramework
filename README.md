These files get you started with a Microsoft Bot Framework "Hello World" chatbot Heroku Node.

The app is based on the MBF document <a href="https://docs.botframework.com/en-us/node/builder/overview/">version</a> and an earlier SarahSays <a href="https://blogs.msdn.microsoft.com/sarahsays/2016/06/01/microsoft-bot-framework-part-1/">version</a>.

One needs a Microsoft Account (I've had a Hotmail account since ages), then an <a href="https://portal.azure.com/">Azure Portal</a> account.

Then go to <a href="http://www.botframework.com">Microsoft Bot Framework</a> and sign in with your Microsoft Account here, too. Register a bot. When you click Edit to edit the bot configuration, click "Manage Microsoft App and password" and make sure that the <a href="https://apps-dev.microsoft.com">Application Registration Portal</a> picks up your Bot Framework AppId. The APR has the ApplicatiuonId for the bot (in the app.js, it is MY_APP_ID). Click "Generate New Password" to do just that. Copy as it is "MY_APP_PASSWORD in app.js.

Enter these two keys on the Heroku Settings page Reaveal Config Vars.

For node on Heroku, one needs to set the port up as done in app.js. 

The Heroku end point is the ned point that goes on the Microsoft Bot Framework configuration (something like https://your_bot_handle.herokuapp.com/api/messages) where the Bot handle is given on the MBF page (it is somethinglike a lowercase version of the MBF name of the bot).

"Test connetion to your bot" gives the response "Accepted" if the Heroku account is recognised (but it does not mean that the bot is working).
