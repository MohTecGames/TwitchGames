===============================================================================
                   TWITCH SPACE SHOOTER PRO (ULTIMATE)
==============================================================================

[ DESCRIPTION ]
A high-octane, Twitch-integrated space shooter designed for streamers. 
The game allows viewers to interact via Twitch chat and can be fully 
customized through URL parameter injection.

--------------------------------------------------------------------------
[ EASY CONFIGURATION ]
------------------------------------------------------------------------------
Instead of manually typing long URLs, use the provided URL Maker tool:

URL Maker: SpaceV4URLMaker.HTML
(e.g., generator.html)

-----------------------------------------------------------------------------
[ PLAYER GUIDE - TWITCH CHAT ]
-------------------------------------------------------------------------------
Use these commands in the Twitch chat to help the pilot:

u / d         -> Move Ship UP / DOWN
s1 / s2 / s3  -> SHOOT (Single / Spread / Wide)
ult           -> ULTIMATE BLAST (60s Cooldown)
gamestart     -> Restart Game

-------------------------------------------------------------------------------
[ STREAMER GUIDE - KEYBOARD ]
-------------------------------------------------------------------------------
Play manually using these keys:

W / S         -> Move Up / Down
SPACE         -> Single Shot
E             -> Spread Shot
D             -> Wide Shot
Q             -> Ultimate Blast

--------------------------------------------------------------------------------
[ ADMIN SETUP: URL INJECTION ]
-------------------------------------------------------------------------------
You can fully customize the game without touching the code by adding 
"Parameters" to the end of your URL.

[ 1. PLAYER PARAMETERS ]
--------------------------------------------------------------------------------
?channel=NAME  -> Connects to a specific Twitch user.
?ship=URL      -> Replaces the ship with a custom PNG link.
?emote=URL     -> Injects an emote into the ship's cockpit.
?emoteX=0.0    -> Horizontal position (0.0 = Left, 0.5 = Center, 1.0 = Right).
?emoteY=0.0    -> Vertical position (0.0 = Top, 0.5 = Middle, 1.0 = Bottom).

[ 2. ENEMY PARAMETERS ]
--------------------------------------------------------------------------------
Target specific enemies by using their ID number (1 through 5).
Example: Use "e1" for Enemy 1, "e2" for Enemy 2, etc.

?e1=URL        -> Replaces the image for Enemy 1.
?e1_emote=URL  -> Replaces the emote for Enemy 1.
?e1_ex=0.5     -> Horizontal position of Enemy 1 emote (0.0 to 1.0).
?e1_ey=0.5     -> Vertical position of Enemy 1 emote (0.0 to 1.0).

-------------------------------------------------------------------------------
[ IMPORTANT NOTES ]
-------------------------------------------------------------------------------------------
* FALLBACKS: If you leave a parameter out, the game automatically 
  uses the built-in defaults.
* EMOTE POSITION: Use decimals (like 0.5) for X and Y. These are 
  relative to the object's size.
* IMAGE REQUIREMENTS: For the "Cockpit" effect, your Ship PNG should 
  have a transparent area where the pilot sits.
* ASSETS: Ensure all local .png files (Enemy1, Enemy2, etc.) are 
  located in the same folder as this HTML file.

================================================================================
