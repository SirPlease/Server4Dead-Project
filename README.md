# < 0 > | **The Server4Dead Project**

<== IMPORTANT NOTICE DON'T IGNORE THIS OKAY?! ===>  
<------------------ **LINUX SUPPORT ONLY** ------------------>  
< This means Windows is not Supported, so don't ask~ :smile: >
> **Project's Purpose:**

This Project's purpose is to make it very easy to get Servers ready for people interested in hosting their own servers for L4D2.  
Feel free to contact me on [Steam](http://steamcommunity.com/id/SirPlease/) regarding the project.  
Also, definitely take a look at [Issues](https://github.com/SirPlease/Server4Dead-Project/issues) to see what's being worked on and or discussed, or to simply request for something to be added to the Project.

> **Recommended Server Specifications:**
* **OS:** Ubuntu 64Bit.
* A Dedicated Server Space, do not use shared resources. (A proper VDS will work just fine)
  * Gameservers are usually hosted in a Shared Environment, thus not recommended. 
* A modern CPU, if you're planning on increasing the tickrate I would aim for a solid 3GHz CPU at minimum.
* DDoS Protection to absorb volume attacks and to filter out malicious traffic.

> **Solid Server Hosts (In My Experience):**
* NFOServers (**for US**, mostly)
  * High Quality VDS and Dedicated Machines.
  * Solid DDoS Protection.
    * Comes for free, included in the price for VDS/Dedicated Server. 
  * Very knowledgeable and Quick Support, they know what they're talking about.

* OVH (**for EU**, mostly)
  * High Quality Dedicated Machines for Dirt Cheap.
  * One of the best DDoS Protection services (if not the best) you can get.
    * Comes for free, included in the price for Dedicated Servers. 
  * Solid Network, low latency.

- - - -
# < 1 > | **Project Current Status**

> **Completed:**
* **Instructions** for setting up your **Dedicated Server** from Scratch.
* **Instructions** for easy Server starting, rebooting and stopping.
* **Tickrate Enabler**, along with Instructions.
* **Sourcemod**, **Metamod**, **Stripper:Source** Package.
* **Extensions**, **Gamedata**, **Competitive Preperation** Package.
* **Sourcemod Anti-Cheat** Pre-configured Package.
* **Optimized Server.cfg:** 
  * Perfect for both "Vanilla" and Competitive Servers. 
  * Easy to understand, as everything is explained within the Server.cfg.
  * Easy to modify to work with **30**, **60**, **100**, **128** or any other Tickrate.
* **Competitive Configs:**
  * **ZoneMod** [1.6](https://github.com/SirPlease/ZoneMod) (1v1, 2v2, 3v3, 4v4)
  * **Apex** [1.1.2](https://github.com/SirPlease/Apex) (4v4) 
      * Includes **Apex Hunters** (1v1, 2v2, 3v3, 4v4)

> **Coming up / In Progress:**
* Additional Competitive Configs.
* Instructions for protecting your Server from small DoS attacks that slip past DDoS filtering. 
  * **Low Priority: as these are filtered by any decent Host that focuses on Game Server with Dedicated Servers**

- - - -
# < 2 > | **F.A.Q.**

> **I'd like to make a suggestion for the Project!**

> **Something isn't working and the F.A.Q. doesn't provide answers either!**

Both of these can be requested/reported in Github's issue tracker for this Project.  
You can do this [**here**](https://github.com/SirPlease/Server4Dead-Project/issues).

> **I've installed the Tickrate Enabler and set my tickrate to 101 or higher, but on the net_graph the bottom value will still be 100!**

This is because it's a hardcoded limit in the client, but don't worry, it's only a visual thing.  
The two middle values on net_graph show you what you're actually getting from the Server.

> **I've installed the Tickrate Enabler, but one or both the middle values aren't reaching the Tickrate set**

First, make sure that you've properly adjusted your rates in the server.cfg as well.  
If everything is set correctly check if the "**sv**" (check the net_graph) isn't struggling to stay above the Tickrate's value, as this will decrease the amount of updates clients are getting from the Server.  
Regarding updaterate, this will only be a client problem if the client has a laggy connection to the Server and is dropping packets.  

The amount of commands a client can send to the Server is limited to the client framerate.  
If you're only getting 60fps, you'll never have an actual cmdrate of above 60.
