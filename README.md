# NO SQLITE SUPPORT ATM #

This requires mySQL or any other **Database** server...


# REQUIREMENTS:

1) Node.js (https://nodejs.org/en/download/ `ver 8.4+`)

2) Discord.js (`npm install discord.js@11.6.2` « should be `ver 11.3+`) 

3.1) ~~SQLite (`npm install sqlite@3`) ~~

3.2) Optional: mySQL (`npm install mysql@2.18.1`) 

→→ if you have a database installed, you can enable it through config (instead of using sqlite)

4) File-System (`npm install fs`) 

5) Request (`npm install request`) 

6) Bot Token: https://discordapp.com/developers/applications/me  

7) And assign bot access to your server: https://finitereality.github.io/permissions/?v=0
-with **Admin** role access, or... permissions to manage roles, channels, and messages... it's your bot, so it is safe!

<hr />

# SETTING IT UP:

1. Download `Node.js` (you probably have it already if running RocketMap/Monocle)

2. Run command: `git clone https://github.com/JennerPalacios/disc_tempRole.git`, once done cloning, open the folder.

3. Open command prompt in this location or click on the handy batch file: `0---start-cmd-here---0` and type the following commands:
   * `npm install discord.js@11.6.2` and
   ~~* `npm install sqlite@3` and~~
   * `npm install fs` and
   * `npm install request`

4. Create an applicaiton and get the your bot's secret token, and application ID at:
   * https://discordapp.com/developers/applications/me 

5. Get your application/bot to join your server by going here:
   * https://finitereality.github.io/permissions-calculator/?v=0
   * Check the boxes for whatever level of power (permissions) you want your bot to have
     * Minimum requirements: manage roles, mannage channels, and manage messages
     * Manage roles, it will only be able to manage roles that are **below** his role/permissions
   * Use the URL that page generates and go to it, and you will be asked to log into your discord, have **Admin** access in order to get the bot to join that server.

5. Fill out the information needed in `files/config.json` (use example or spm as example), and launch each module!

<hr />

# LAUNCHING IT:

Using command prompt or bash: `node TempRoles.js`

-If you close that window, the bot connection will be terminated!

**Optional**: you can install pm2 to have it run in the background

<hr />

# PM2:

PM2 allows you to run processes in the background, you can access PM2 from anywhere, but for a process to start it needs to come from the folder where the file is located.

`npm install pm2 -g`

`pm2 start TempRoles.js`

To modify the file and keep bot up-to-date (auto reloading):

`pm2 start TempRoles.js --watch`

Other Commands:

`pm2 log` (display log)

`pm2 list` (display a list of running processes)

`pm2 stop NAME/ID`
