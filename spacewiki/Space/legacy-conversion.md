# Converting from legacy
This guide will effectively walk you through converting from Space 8.1 and below, to Space 8.2 and above

Note: It is only necessary to do all of these instructions once.

## Backwards compatibility
* All inventory based items will be converted into their newer versions
* All placed blocks will break (eg: quantum workbench, suit fabricator, airlocks, etc). This can be resolved by picking them up before converting, and they will be converted too.

## Steps to convert
1. Firstly, and most importantly, create a backup of either the server or Space alone using "/space backup". This is necessary because all Space configuration files have been reworked to have nicer formatting, more options, and a few more files have been added.
2. Stop your server if you haven't already.
3. Delete ALL space configuration files **except your database.yml**
4. Replace the old Space jar, with the latest Space jar from Spigot.
5. Restart your server.
6. Configure the plugin however you like, since you will now be running on fresh configuration files. **You can not replace these with your old configuration files.**

## Issues
If you have any "stuck" legacy blocks, please use the debug wand (Attained from "/space cheat") to forcefully remove them.

If you have any strange texture issues, please reset your resource pack cache. Instructions can be found [here](https://github.com/Z4OLLIEZ4/Space/wiki/Resource-Pack)