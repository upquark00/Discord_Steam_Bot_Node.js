# Simple Discord Bot in Node.js

This is the Node.js version of the Discord_Steam_Interface Bot found here:  
[Discord_Steam_Interface Bot (Python edition)](https://github.com/upquark00/Discord_Steam_Interface)

This project creates a bot intended to discover and display a Discord user's 
current activity by

(a) Checking for an active session in Steam, a major gaming platform, and importing 
details about the user's active game, if applicable.  

Status will be translated as follows:  

   | STEAM STATUS | STEAM STATE | DISCORD STATUS |
   |-----------|:-----------:|-----------:| 
   'Offline'           |      0      | 'Offline'
   'Online'            |      1      | 'Online'
   'Busy'              |      2      | 'dnd'
   'Away'              |      3      | 'Idle'
   'Snooze'            |      4      | 'Idle'
   'Looking to trade'  |      5      | 'Online'
   'Looking to play'   |      6      | 'Online'

(b) If no active Steam session is found, information about the user's currently 
active window will be returned instead. 

### Requirements
    
    (0) A system which runs Node.js. (See below for installation)
    
	(1) a Steam ID, obtainable via the Steam client under View > Settings. 
	
	(2) a Steam API Key, which can be found here: 
    	https://steamcommunity.com/dev/apikey
    	
	(3) a Discord bot token, which can be created in the Discord Developer portal: 
    	https://discordapp.com/developers/applications/

### Check Dependencies  
Node.js is required to run this bot. See it's already installed by entering the into 
 your system's command line: `node -v`.
 
 A response such as `v12.13.0` indicates the version of Node currently installed. 
 A response such as `'node' is not recognized as an internal or external command, 
 operable program or bacth file` indicates you need to install or re-install. 
  
If necessary, install Node.js here: [Download Page](https://nodejs.org/en/download/)  

To install discord.js by using `npm install discord.js`

If interested in modifying any functionality, please read the Discord.js documentation before moving on: 
[Read the docs](https://discord.js.org/#/)