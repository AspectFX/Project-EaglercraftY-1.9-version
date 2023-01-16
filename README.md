# Project-EaglercraftY-1.9-version
This project wil have the official Code of minecraft  1.9.4 and this respository will be updated
(rip-off of 1.8.8 code)
# EaglercraftY?

### Note: we will be transitioning away from Eaglercraft being standalone 'free browser minecraft' to Eaglercraft being a bukkit/bungee plugin for servers to allow 'online access' to players who register with a command as their real online-mode Minecraft account on the server. Server owners can still elect to set `online-mode=false` in their server.properties to allow free login but now that's their legal screw up instead of mine'
![Preview-Build-of-1](https://user-images.githubusercontent.com/67106394/210432989-0d541ef1-bd39-4b90-9bb1-c0ffae1b9c3e.jpg)



### Official Demo URL: (No link yet)

### Download Locally:(or Hmtl file)

## What is Eaglercraft?

Eaglercraft is real Minecraft 1.9 that you can play in any regular web browser. That includes school chromebooks, it works on all chromebooks. You can join real Minecraft 1.9 servers with it through a custom proxy based on Bungeecord.

## How to make a server

### If replit is acceptable, you can use this:

### (there No replit yet for 1.9 version)

### Manual setup instructions:
1. **Check if Java is installed.** You can download it from [https://www.java.com/en/download/](https://www.java.com/en/download/)
2. Download the [stable-download/stable-download-new.zip](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/stable-download-new.zip) file from this repository
4. Extract the ZIP file you downloaded to a new folder
5. Open the new folder, go into the `java/bungee_command` folder
6. In Windows, double-click `run.bat`. It should open a new terminal window  
![run.bat](https://i.gyazo.com/2b0f6b3e5b2e5a5a102c62ea5b6fba3f.png)  
**Some computers may just say 'run' instead of 'run.bat', both are correct**
7. On macOS or Linux, google how to open the terminal and use the `cd` command to navigate to `java/bungee_command`  
Then, in that folder, run `chmod +x run_unix.sh` and then run `./run_unix.sh`. It should start the same server
8. Go to the other `java/bukkit_command` folder that was also extracted from the ZIP
9. Again, on Windows, double-click `run.bat` in the folder. It should open a second terminal window.  
Keep both the first and second terminal window you opened, just minimize them don't close
10. Again, on macOS or Linux, repeat step 7 except in the `java/bukkit_command` folder
11. **Your server is now ready.** Download and open [stable-download/Offline_Download_Version.html](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/Offline_Download_Version.html)
12. Go to 'Multiplayer' from the main menu. Select 'Direct Connect', type `127.0.0.1:25565` and press 'Join Server'
13. **It should allow you to connect, if not, check the two terminal windows for errors**
14. If you are okay with regularly checking for updates to [Offline_Download_Version.html](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/Offline_Download_Version.html), you are now finished
15. If you are playing with friends and want a shared website that can be updated, see the `stable-download/web` folder
16. To install, create a website and upload the contents of `stable-download/web` to the URL you want to have Eaglercraft on
17. **The 'web' folder will not work if you open it in your browser locally! If you see 'file:///' in the URL you are doing it wrong. You need to upload the folder to an HTTP or HTTPS server and access it over the internet via http:// or https://. The game will not load otherwise, this is not a bug**
18. To modify the default list of servers, download [servers_template.dat](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/servers_template.dat) and open it in [NBTExplorer](https://github.com/jaquadro/NBTExplorer/releases). Make your changes and then save
19. **If you can't install NBTExplorer, try [WebNBT](https://irath96.github.io/webNBT/)**
20. Upload your modified `servers_template.dat` to [base64encode.org](https://www.base64encode.org/) and press 'Encode'.
21. Download and open the encoded file, copy and paste the text in the file back between the quotes in `index.html` at line 21 (or 22) in place of the old text that also begins with `CgAACQAHc2Vydm` between the quotes
22. **To create a link to your site that automatically joins the server,** add a `?server=` variable to the URL, like (for example): [https://g.eags.us/eaglercraft/?server=127.0.0.1:25565](https://g.eags.us/eaglercraft/?server=127.0.0.1:25565) will automatically join `ws://127.0.0.1:25565/` as soon as the player finishes setting their username and skin
23. To change your server's MOTD and icon, edit the `motd1:` tag of the listener config in `java/bungee_command/config.yml`, and replace `server-icon.png` in the folder where the config file is. Use `&` to add color/formatting codes. The server list will downscale your icon to 64x64 pixels
24. You can give your MOTD multiple lines, add a `motd2:` to define a second line
25. **For an animated MOTD and icon, install EaglerMOTD: [https://github.com/LAX1DUDE/eaglercraft-motd/](https://github.com/LAX1DUDE/eaglercraft-motd/)**
26. To add some bukkit plugins, download the plugin's JAR file for CraftBukkit 1.5.2 and place it in `java/bukkit_command/plugins`
27. To add some bungee plugins, download the plugin's JAR file and place it in `java/bungee_command/plugins`
28. See [https://github.com/LAX1DUDE/eaglercraft-plugins/](https://github.com/LAX1DUDE/eaglercraft-plugins/) to download some supported plugins
29. To add `/login` and `/register`, install [AuthMe](https://github.com/LAX1DUDE/eaglercraft-plugins/tree/main/AuthMe) and carefully [read it's documentation](https://github.com/AuthMe/AuthMeReloaded/wiki) to set it up correctly
30. **To ban a username on Eaglercraftbungee, use:** `eag-ban <username>`
31. **To ban an IP on Eaglercraftbungee, use:** `eag-ban-ip <ip>`, or `eag-ban-ip <name>` to ban the IP of a player automatically
32. To ban a range of IP addresses, use slash notation to define a subnet. Example: `eag-ban-ip 192.168.0.0/8`
33. To ban users by wildcard (\*) use: `eag-ban-wildcard <text>*` or `eag-ban-wildcard *<text>` or `eag-ban-wildcard *<text>*`
34. **You can edit bans.txt in your EaglercraftBungee folder, the server automatically reloads the file when it is saved**
35. To ban users by regular expression, use: `eag-ban-regex <regex>` with a regular expression to match the username in **lowercase**
36. **If you use /op on your server, keep in mind that if you "/op LAX1DUDE", a player joining as 'laX1DUDE' or 'LaX1dUdE' or 'lax1dude' will all have /op too. To solve this problem, force all operators to only be able to join with all lowercase ('lax1dude') letters in their usernames by moving 'BitchFilterPlugin.jar" into "java/bukkit_command/plugins" and then register every op username lowercase**
37. To connect to your server through a `ws://` or `wss://` URL instead of `ip:port`, set up [nginx](https://nginx.org/) as a reverse proxy to the `ip:port` of you EaglercraftBungee server you want the URL to connect to. Use a location URL template with the `proxy_pass` directive.
38. Eaglercraft uses port 80 for IP connections by default, typing `127.0.0.1` is the same as typing `ws://127.0.0.1:80/`
39. To forward a client's remote IP address from a request on nginx to EaglercraftBungee for enforcing IP bans, set the `X-Real-IP` header on the request to websocket when it is proxied
40. To make a custom resource pack for your site, clone this repository and edit the files in [lwjgl-rundir/resources](https://github.com/LAX1DUDE/eaglercraft/tree/main/lwjgl-rundir/resources).
41. When you are done, navigate to [epkcompiler/](https://github.com/LAX1DUDE/eaglercraft/tree/main/epkcompiler) and double-click `run.bat`. Wait for the window to say `Press any key to continue...` and close it. Then, go to `../javascript` in the repository and copy `javascript/assets.epk` to the `assets.epk` on your website
42. If you're on mac or linux, navigate to the epkcompiler folder via `cd` and run `chmod +x run_unix.sh` and then `./run_unix.sh` to do this, then copy the same `javascript/assets.epk` to the `assets.epk` on your website

## Singleplayer?
(no singleplayer yet)
## How does it work?

Eaglercraft uses the decompiled source code of the official build of Minecraft 1.5.2 direct from Mojang. It is decompiled by [MCP](http://www.modcoderpack.com/) and then recompiled to Javascript using [TeaVM](https://teavm.org/). Therefore it can join real Minecraft 1.9 servers, as it is really running Minecraft 1.9 in the browser. However, due to security limitations in modern browsers, it must use javascript Websocket objects for multiplayer instead of direct TCP connections to it's servers. A modified version of Bungeecord is included with Eaglercraft which accepts browser HTTP Websocket connections from Eaglercraft clients and unwraps the streams internally to regular TCP so they can be forwarded to regular Bukkit servers with no plugins. For graphics, a custom GPU compatibility layer allows Mojang's fixed function OpenGL 1.3 based rendering engine to render directly to an HTML5 WebGL 2.0 canvas on the page with minimal changes to the source, preserving the game's graphics to look exactly the same as desktop vanilla Minecraft 1.9 (comming soon)

## Issues?
(discord  channel will be Made a Later Date)

## EaglercraftBungee

EaglercraftBungee translates WebSockets to a raw Minecraft 1.9 TCP connection. It is just regular BungeeCord with more `config.yml` options, and a built in plugin for syncing people's custom skins between clients so people can see each other's skins

**Enable** `forward_ip` **and pass a X-Real-IP header from your proxy to use rate limiting and IP bans on a URL**

Nginx example: add `proxy_set_header X-Real-IP $remote_addr` to your proxy configuration

**The server has built in DoS protection, reset it via typing 'eag-ratelimit reset' in the bungee console**

```yaml
ratelimit:
  ip:
    enable: true
    period: 90
    limit: 60
    limit_lockout: 80
    lockout_duration: 1200
    exceptions: []
```

- `enable` enable rate limiting

- `period` and `limit` set the number of requests (`limit`) can be made in (`period`) number of seconds

- `limit_lockout` and `lockout_duration` set the number of requests (`limit_lockout`) that can be made in (`period`) seconds before the IP is blocked for `lockout_duration` number of seconds

- `exceptions` a list of IP addresses that should never get rate limited. **Local IPs like 127.0.0.1 and 192.168.\*.\* and such are set as exceptions by default**

**To develop a plugin, download [stable-download/java/bungee_command/bungee_dist.jar](https://github.com/LAX1DUDE/eaglercraft/blob/main/stable-download/java/bungee_command/bungee-dist.jar) and add it to the Build Path of your Java IDE. Develop the plugin just like a regular BungeeCord plugin, see [EaglerMOTD](https://github.com/LAX1DUDE/eaglercraft-motd/) for an example.**

**Test your plugin by exporting it as a jar and putting it in the '/plugins' directory of EaglercraftBungee and then clicking 'run.bat'**

### New Events:

- **[net.md_5.bungee.api.event.WebsocketMOTDEvent](https://github.com/LAX1DUDE/eaglercraft/blob/main/eaglercraftbungee/src/main/java/net/md_5/bungee/api/event/WebsocketMOTDEvent.java)**: Triggered when a client or website requests the MOTD

- **[net.md_5.bungee.api.event.WebsocketQueryEvent](https://github.com/LAX1DUDE/eaglercraft/blob/main/eaglercraftbungee/src/main/java/net/md_5/bungee/api/event/WebsocketQueryEvent.java)**: Triggered when a client or website requests a query. This happens when a site opens a text WebSocket to a listener and sends a single string `Accept: <query>` packet. Can be used to provide additional custom statistics to server list sites supporting integrated WebSocket queries

**Register event handlers using the standard BungeeCord** `@EventHandler` **annotation in your** `Listener` **class**

## Installing (detailed)

If you want to use this project but don't want to compile it from scratch, download [stable-download/stable-download-new.zip](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/stable-download-new.zip) and extract

Within stable-download-new.zip there is a 'java' and a 'web' folder. Upload the contents of the web folder to your web server. **The web folder will not work if it is opened locally via file:///, it needs to be opened on an http:// or https:// page. Try [this extensions](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb/) if you are on chrome or if that's not possible then download the alternative single-file html [offline version](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/Offline_Download_Version.html) that does work on file URLs.** If you use this alternative version, please make sure you and your peers keep your copies up to date by regularly downloading any newer versions of the html file at [this link](https://github.com/LAX1DUDE/eaglercraft/blob/main/stable-download/Offline_Download_Version.html) to avoid getting stuck with a version that has a game-breaking glitch or mistake. The eaglercraft bungeecord executable is in the java/bungee_command folder along with the sample configuration file and a run.bat script to launch it. CraftBukkit for minecraft 1.5.2 configured to work with the eaglercraft bungee executable is in java/bukkit_command. The available version of Spigot 1.5.2 has a bug when used with bungee so you are limited to CraftBukkit and CraftBukkit plugins only on your servers

**Here are some Bukkit plugins compatible with Eaglercraft: [https://github.com/LAX1DUDE/eaglercraft-plugins](https://github.com/LAX1DUDE/eaglercraft-plugins)**

To play the game, launch the run.bat script in both the bungee_command and bukkit_command folders. Then navigate to the URL where the contents of the web folder ended up. The game should load without any issues. Go to the Multiplayer screen and select 'Direct Connect'. **Type 127.0.0.1:25565.** Press connect or whatever and enjoy, the default port configured in the bungeecord config.yml is 25565 instead of 80 to avoid any potential conflict with the local web server or the OS (and linux desktop users can't use port numbers under 1024 without sudo).

**The default behavior in Eaglercraft if no :port is provided when connecting to a server is to use port 80, not port 25565. This is so the game's multiplayer connections in a production environment do not default to a port that is currently blocked by any firewalls. Also this enables you to use Cloudflare and nginx to create reverse proxy connections on your site to host multiple servers on the same domain using different ws:// URLs for each socket.**

If you want SSL, set up [nginx](https://www.nginx.com/) as a reverse proxy from port 443 to the port on the bungeecord server. You can very easily configure SSL on an nginx virtual host when it is in proxy mode, much more easily than you could if I created my own websocket SSL config option in bungee. To connect to a server running an SSL websocket on the multiplayer screen, use this format: `wss://[url]/`. You can also add the :port option again after the domain or ip address at the beggining of the URL to change the port and connect with SSL. **If you set up the Eaglercraft index.html on an https:// URL, Chrome will only allow you to make wss:// connections from the multiplayer screen. It is a security feature in Chrome, if you want to support both ws:// and wss:// you have to host the Eaglercraft index.html on an http:// URL**. The best advice I have for security is to use Cloudflare to proxy both the site and the websocket, because you can use http and ws on your servers locally and then you can configure cloudflare to do the SSL for you when the connections are proxied. And it conceils your IP address to the max and you can also set up a content delivery network for the big assets.epk and classes.js files all for free on their little starter package

**To change the default servers on the server list, download [stable-download/servers_template.dat](https://github.com/LAX1DUDE/eaglercraft/raw/main/stable-download/servers_template.dat) and open the file with NBTExplorer (the minecraft one). You will see the list of default servers in a 'servers' tag stored as NBT components, and you can edit them and add more as long as you follow the same format the existing servers have. When you're done, save the file and encode the file back to base64 using the upload option on [base64encode.org](base64encode.org), then download the encoded file and open it and replace the base64 between the quotes on line 8 of your index.html with the new base64 in the encoded file you downloaded.**

There is a plugin hard coded into the bungeecord server to auto synchronize the eaglercraft profile skins between players and worlds

You should probably use a plugin like [AuthMe](https://dev.bukkit.org/projects/authme-reloaded/files/682502) to keep griefers from logging in to other people's profiles

## Compiling

To compile for the web, run the gradle 'teavm' compile target to generate the classes.js file.

To complile to regular desktop Java for quick debugging, using native OpenGL for rendering instead of WebGL:
- Create a new empty eclipse project
- Link the src/main/java and src/lwjgl/java as source folders and add the jars in lwjgl-rundir as dependencies
- Create a run configuration and add a jvm argument pointing to the lwjgl natives folder (lwjgl-rundir/natives) like this: `-Djava.library.path=natives`, and make sure the working directory for the run configuration is the lwjgl-rundir folder.


To modify the game's resource pack (javascript/assets.epk), view the readme in the [/epkcompiler](https://github.com/LAX1DUDE/eaglercraft/tree/main/epkcompiler) directory

this project is just a proof of concept to show what can be accomplished when using TeaVM to cross compile an existing java program to javascript. It is not very fast or stable, and the only real useful portion is the emulator code which creates a makeshift fixed function OpenGL 1.3 context using webgl (based on OpenGL 3.3) operational in the browser. Maybe it can be used to port other games in the future.

## Contributing

All I really have to say is, tabs not spaces, and format the code to be like the eclipse auto format tool on factory settings, but also run-on lines of code long enough to go off the screen and single line if statements and other format violations in that category are welcome if it helps enhance the contrast between the less important code and the more important code in a file. Don't commit changes to `javascript/classes.js` or `javascript/assets.epk` or anything in `stable-download/`. I'll recompile those myself when I merge the pull request.






## Snapshots of 1.9.4 version (in progress development build)













## Free Update Snapshots of the Improved Gui (Photoshopped version)







## Free Update List for New stuff
May include
1.new eletrya 
2. New End cities
3.adding a Warden
4. new Blocks (sulk,Caystic,Acacia Boat with Chest,Allay Spawn Egg,Birch Boat with Chest,Bucket of Tadpole,Dark Oak Boat with Chest
Disc Fragment
Echo Shard
Frog Spawn Egg
Frogspawn
Goat Horn
Jungle Boat with Chest
Mangrove Boat
Mangrove Boat with Chest
Mangrove Button
Mangrove Door
Mangrove Fence
Mangrove Fence Gate
Mangrove Leaves
Mangrove Log
Mangrove Planks
Mangrove Pressure Plate
Mangrove Propagule
Mangrove Roots
Mangrove Sign
Mangrove Slab
Mangrove Stairs
Mangrove Trapdoor
Mangrove Wood
Mud
Mud Brick Slab
Mud Brick Stairs
Mud Brick Wall
Mud Bricks
Muddy Mangrove Roots
Music Disc
Oak Boat with Chest
Ochre Froglight
Packed Mud
Pearlescent Froglight
Recovery Compass
Reinforced Deepslate
Sculk
Sculk Catalyst
Sculk Shrieker
Sculk Vein
Spruce Boat with Chest
Stripped Mangrove Log
Stripped Mangrove Wood
Tadpole Spawn Egg
Verdant Froglight
Warden Spawn Egg

end of List



