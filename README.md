# Slime Bot

![alt text](king_slime_solo.png)

# A discord bot built for Maplestory M using discord.js. 

 - Utilizes **Enmap** for per-server configurations and **Cron** for scheduled messages.
  

## Functionalities:

- 15 minute reminders for afternoon and nighttime expeditions! Customize message and channel it sends to.
  
- 15 minute reminder for guild fort. Customize message and channel it sends to.

- Reminder for banquet. Customize time, message and channel it sends to.

- Greets new guild members. Customize private welcome greeting.

- !fuse command to help with fusing - includes cost and data (treasure pulls, powder, equips, potentials, pba ranges)

- !jewel command for jewel data.

- !team command for organizing expeditions.

- !party command for organizing SF/leech parties.

## Commands: 

- !fuse - helps with fusing costs.

- !jewel - jewel data

- !team - organizing expeditions

- !party - organizing parties

- !help - shows bot's commands.

- !showconf - shows current configurations (GM only)

- !setconf - edit configurations (GM only)
  
- !resetconf - resets configurations to default settings (GM only)


# IMPORTANT - please give yourself the role of 'GM' in order to start using admin commands such as !setconf and !showconf.

## Configuration Help:

### What are configs and why they are important
 
- Every guild discord is different - they have their own specific channels, banquet times, GMs want their own reminder messages, etc etc. Configurations basically help you edit all of these to your liking.

### Configuration Keys and Value

- There are 2 parts to my configurations: **keys and values**.

- The **key** is the type of configuration. 

- Some examples of **keys** include: 'expoMessage', 'banquetTime', 'expoChannel', & 'privateMessage'.

- The **value** is the value of that particular **key**, and this is what you will be changing. 

- For example, the default **value** of the **key** 'expoChannel' is set to 'general'. This means that my expedition reminders will be sent to the channel called 'general' by default. 

- If you don't have a channel called 'general', or want me to send expedition reminders to a different channel, let's say a channel called 'expedition-reminders', you would change the **value** of expoChannel to 'expedition-reminders'."
                  
### Changing values
- To change the value of a key, type !setconf followed by the **key** and then the **value** you want.

- For the example above, simply type **!setconf expoChannel expedition-reminders**. This will set my expedition reminder messages to send only to the channel **expedition-reminders**.

- You can then type **!showconf** to view your changes. Simple enough, right?

- If you're not getting reminders from me, there is probably an error in your configs (check spelling and/or letter casing). 

- Now go edit your configs!
  
### Keys and their functionalities

- **adminRole** : Only people with this role can use admin commmands such as !setconf. Defaults to 'GM', so when using the bot for the first time, please assign yourself the role of 'GM' to start using. You can change this to your liking later.

- **privateMessage**: private DM sent to new guild members joining discord.

- **expoChannel**: channel for expedition reminders.

- **expoMessage**: this message will be sent to expoChannel **15 minutes** prior to expeditions. 

- **banquetTime**: the time you want me to remind your guild about banquet.

- **banquetChannel**: channel for banquet reminders.

- **banquetMessage**: message sent to banquetChannel.

- **fortMessage** : message sent to fortChannel.

- **fortChannel** : channel for guild fort reminders.

- **checkInChannel** : channel to use !team command in.


### Default Configurations

- **adminRole** : GM <-- ***important: make sure to assign 'GM' role to yourself so you can use !setconf.***

- **privateMessage** : Hi there, welcome to our discord! Please change your nickname to your in-game IGN. Type !help for my list of commands!

- **expoChannel** : general

- **expoMessage** : @everyone Expeditions are starting in 15 minutes! Good luck!

- **banquetTime** : 00 18 <-- ***important: banquetTime is formatted by [minute][hour] in server time, so 00 18 = 6pm server time. Keep this in mind when setting your own banquetTime!***

- **banquetChannel** : general

- **banquetMessage** : @everyone Banquet is starting in 15 minutes!

- **fortMessage** : @everyone Guild fort is starting in 15 minutes!

- **fortChannel** : general

- **checkInChannel** : general


### Discord Server for Updates

**If you are using this bot, please join this discord server for Slime Bot Updates** : https://discord.gg/rkwNAxj;

**Please visit the website at https://www.slimebot.org for more info**

### How to Set Up

- ** After cloning the repo, remove the node_module directory and package-lock.json file
- ** If you're on Linux, download Node v10.18.0 and Python "sudo apt-get install python-is-python3"
- ** Run npm install, and you're good to go
- ** IF it does not compile, you might have to remove the node_module and package-lock.json and install once again.
- ** Run npm run start
