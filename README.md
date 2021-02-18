# SA-MP Tools
Useful tools for a SA-MP server

## Setup
To setup a SA-MP Server, you need to download it from [here](https://www.sa-mp.com/download.php "Official Download").
I'm assuming you have SA-MP client installed but if you don't, you just need to download it from the same site, although there are some additional requirements:
* Downgrade your game to Patch 1.0
* If you're using steam version, keep in mind that the executable needs to be named `gta_sa.exe` and not `gta-sa.exe`.

Getting back to the server, first thing you need to do is edit the config file. The config file looks like this:
```
echo Executing Server Config...
lanmode 0
rcon_password changeme
maxplayers 50
port 7777
hostname SA-MP 0.3 Server
gamemode0 grandlarc 1
filterscripts gl_actions gl_realtime gl_property gl_mapicon ls_elevator attachments skinchanger vspawner ls_mall ls_beachside
announce 0
chatlogging 0
weburl www.sa-mp.com
onfoot_rate 40
incar_rate 40
weapon_rate 40
stream_distance 300.0
stream_rate 1000
maxnpc 0
logtimeformat [%H:%M:%S]
language English
```
I'll explain each line below, with prefered values set:
```
echo Executing Server Config... - Nothing important, just leave it like this.
lanmode 0 - If you'll need it you'll figure it out
rcon_password none - Password for admin commands, has to be changed
maxplayers 1 - Maximum player count, set it to 1 if you're playing on localhost
port 7777 - Port of server, this one is default, if you don't have to, don't change it.
hostname My Server - Display name of your server.
gamemode0 grandlarc 1 - Master script that should be ran, more about it in server-readme.txt
filterscripts gl_realtime gl_mapicon my_filterscript - List of additional scripts for your server..
announce 0 - Set to 1 if you're running a public server.
chatlogging 1 - Should chat messages be logged?
weburl https://www.youtube.com/watch/dQw4w9WgXcQ - Your website if you have one.
onfoot_rate 40 - Tick rate when on foot
incar_rate 40 - Tick rate when in a vehicle
weapon_rate 40 - Weapon tick rate
stream_distance 300.0 - What distance is "nearby" for a player?
stream_rate 1000 - No idea
maxnpc 0 - Maximum npc count, i'm not going to talk about them here so keep it as 0;
logtimeformat [%H:%M:%S] - Exactly what it says
language English - Hmm... What could it be...
```

## Scripting

Hold on, i have to save changes

## Useful links

* [Unofficial SA-MP Docs](https://open.mp/docs "open.mp") - The official ones are lost but these are better anyway.
