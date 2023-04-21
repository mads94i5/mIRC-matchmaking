# mIRC-matchmaking

A script made many years ago at the beginning of me self-learning code.
The script was made to make it easier to find matches in Counter-Strike, back when people used IRC to find matches.
It is meant as a script to put on a bot/seperate instance of mIRC and when prompted with the correct commands, it will join a few different IRC channels and start advertising the kind of match you are searching for as well as start messaging people who are advertising something that matches your search. 
You can set up IP and password if you have your own game server and if you search with a server, it will give IP and password to the first person that has an advertisement that matches your search and then stop searching. If you search without a server, the script will request IP and password in a private message and relay that to the private channel that you set up in the script. 
The bot will also ignore any links, as malicious links in private messages was not uncommon.

Note: It is no longer viable as a matchmaking tool as no one really uses IRC to find matches in Counter-Strike anymore since the adoption of CS:GO, which has it's own matchmaking system and popular alternative matchmaking on websites such as faceit.

But it was a tool that was far ahead of its time as matchmaking was not a standard feature in games at the time when I made this script. And I found that it might be worth hosting here as a memento and a display of how I started learning to code.

The code is not beautiful, it's honestly a bit of a mess. But it was functional and was used a lot by me and my friends back when Counter-Strike 1.6 was popular.

How to use script:
1. Put the script in your bot/seperate mIRC instance. (Example: C:/Users/YOURWINDOWSUSER/AppData/Roaming/mIRC/scripts)
2. Edit the script #channelname to fit your private IRC channel.
3. Give the bot +o (operator on your private channel).
4. Now you and your friends with access to your private channel can type commands to the bot.

Below is a description of the commands:
  Type !help in your private channel to see all the commands.

  Type !from <country> to set your country.

  Type !ip <server IP> to set your game server IP.

  Type !pw <server password> to set your game server password.

  Type !<2on2/3on3/4on4/5on5> <on/off> <noobs/low/med/high> <optional text> to start searching for a match. For example if you have a game server and want a 5on5 at high skill: !5on5 on high

  Type !amsg <text> to make the script do an /amsg which sends a message to all channels it's currently on.

  Type !msg <message number> <text> to send a message to a specific person that messaged the bot. The bot will relay all non-spam private messages to the private channel. This command let you communicate with them from other instances of IRC on your private channel.

  Type !giveip <message number> to give the IP and password to a specific person that messaged the bot.

  Type !stop to force the bot to stop searching for a match.
  
