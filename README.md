# Discord Meme Economy Bot
This bot will allow users to create a "meme economy" out of one of their server channels. The meme economy bot allows users to invest, check balances and manage their portfolio.
For more information about the meme economy please visit www.reddit.com/r/memeeconomy.

## Installation
- Ensure `Python 3.5` is installed on your system
- Install `Discord.py` (the python discord API) with the command `pip install discord.py`
- Create an application at https://discordapp.com/developers/applications/ and copy the **TOKEN** from the BOT settings
- Get the Channel ID for the channel you wish to make your meme economy. To do this open the Discord application and go to `User Settings -> Appearance -> Enable Developer`. Right click on the channel and copy the ID.

## Adding the bot to your server
On the Discord Developer page we were just on go to the "App Details" page and copy your "Client ID".
Replace the "CLIENTID" in this link with your ID you just copied and enter the link into your browser: 

    https://discordapp.com/oauth2/authorize?&client_id=CLIENTID&scope=bot&permissions=8 

This should bring you to a page where you can choose what discord server to send your bot to.

## Running your new Bot
In a Terminal window or CMD type:

    python main.py --token YOURTOKEN --channel YOURCHANNELID
    
simply replace "YOURTOKEN" and "YOURCHANNELID" with the token value and channel id respectively.

You should see some output to the console and you should be able to see in your server that your bot is online.
Terminating the script execution will turn the bot offline.

## Notes
Only post that are submitted **after** the bot is online will be eligible for investing in the economy.