# Telephony Channel
Telephony Channel in Microsoft Bot Framework allows you to bind an existing PSTN phone number acquired using Microsoft Teams Phone System with a Bot in Microsoft Bot Framework.

Telephony channel under the hood is built upon Microsoft Speech Services to allow Speech to Text and Text to Speech capabilities crucial for enabling an audio interaction/conversation over phone lines.

Please follow these steps to enable a Telephony channel for your bot.

## Enable Telephony Channel in the bot

Once we have created a speech resource, we are ready to use it and configure it using the information collected in previous sections.

Go to the [Azure portal](https://portal.azure.com) > Bot (Created in previous [step](CreateBot.md)) > Channels

![](images/create-a-bot/c015-click-on-channels.png)

For you to see Telephony as one of the options, your Azure account needs to be whitelisted for the Private Preview by a member of Microsoft Bot Framework team.  If you were whitelisted successfully, you will see the Telephony channel:

![](images/create-a-bot/c016-click-on-telephony.png)

Configure the channel with following information:

* Telephony number - Acquired previously in [provisioning a new phone number for your bot in Azure Communication Services](https://docs.microsoft.com/en-us/azure/communication-services/quickstarts/telephony-sms/get-phone-number)
* Azure Communication Service Access Key and Endpoint - Acquired while [creating a Azure Communication Services Resource](https://docs.microsoft.com/en-us/azure/communication-services/quickstarts/create-communication-resource)
* Cognitive Service Subscription Key - Acquired while [creating the Speech Resource](CreateSpeechResource.md)
* Location for the chosen for the Cognitive Service Speech Resource 
    - Format: WestUS, WestUS2, EastUS, EastUS2, WestEurope, NorthEurupe,SouthEastAsia


![](images/create-a-bot/c017-fill-out-settings-click-save.png)

Click **Save**.

**Next step**:  [Process speech inside of the bot](ProcessSpeechInBotCode.md)
