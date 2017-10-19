# | **Tickrate Enabler**

This part of the Project will focus on modifying the Tickrate on your L4D2 Server.
While everything here is also covered in all the files (server.cfg and srcds file), I'll put it here again.

> **How to Change the Tickrate?**  
> If you're running a VDS or Dedicated Server, all you have to do is change the launch parameters (which in this Project are set by the srcds file)  
> If however you're renting a Gameserver, you will have to ask the Server host to change the launch parameters for you.

**Step 1:** Place the files provided in the correct folder.

**Step 2:** Change the Launch Parameters.
If you're following this Project, simply modify the SRCDS file provided in the ***Dedicated Server Fresh Start*** folder.  
If not, surely you'll know where to find the launch parameters.

If you're going to adjust your Tickrate above 100, you will run into Boomer Vomit Range issues.  
You will need to add "**-frametime 0.037 -frametime_override 0.037**" to the launch parameters to resolve this, make sure to place them after the tickrate parameter.

**Step 3:** Adjust your server.cfg to match your rates accordingly.  
For example: For 128 Tickrate, you'd want these settings:

sm_cvar sv_minrate 128000  
sm_cvar sv_maxrate 128000  
sm_cvar sv_minupdaterate 128  
sm_cvar sv_maxupdaterate 128  
sm_cvar sv_mincmdrate 128  
sm_cvar sv_maxcmdrate 128  
sm_cvar net_splitpacket_maxrate 128000  
sm_cvar fps_max 0  



