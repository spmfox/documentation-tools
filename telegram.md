## Telegram
These are the minimum steps for creating a Telegram bot, adding the bot into a chat, and getting the chat id.

* Open Telegram
* Start a chat with @BotFather
  * Type `/newbot` to start the wizard
  * Once your bot is created, grap the HTTP API key
* Create new chat, or channel
* Invite bot into the chat or channel
* Send any message into the channel
* Go to `https://api.telegram.org/botXXX:YYYY/getUpdates`
  * Replace XXX:YYYY with your HTTP API key for the bot (keep the `bot` part of the URL)
* You should see some JSON output that contains this "chat":{"id": followed by a large negative number
* Copy the entire number, including the "-" symbol, thats your chat id
  * If you've re-used this bot, there may be other entries there from other chats - you'll have to find the right one

Now, not only do you have the chat id but you have your bot created and the bot is inside the chat or channel ready to go.

**Make sure to review your security settings for the chat or channel and the bot.**
