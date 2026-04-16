==========================================================================
                   TWITCH SPACE SHOOTER PRO (ULTIMATE)
==========================================================================

[ DESCRIPTION ]
A high-octane, Twitch-integrated space shooter designed for streamers. 
The game allows viewers to interact via Twitch chat and can be fully 
customized through URL parameter injection.

--------------------------------------------------------------------------
[ EASY CONFIGURATION ]
--------------------------------------------------------------------------
Instead of manually typing long URLs, use the provided URL Maker tool:

URL Maker: 
https://mohtecgames.github.io/TwitchGames/Shooter/SpaceV4URLMaker.HTML 

--------------------------------------------------------------------------
[ PLAYER GUIDE - TWITCH CHAT ]
--------------------------------------------------------------------------
u / d         -> Move Ship UP / DOWN
s1 / s2 / s3  -> SHOOT (Single / Spread / Wide)
ult           -> ULTIMATE BLAST (60s Cooldown)
gamestart     -> Restart Game

--------------------------------------------------------------------------
[ STREAMER GUIDE - KEYBOARD ]
--------------------------------------------------------------------------
W / S         -> Move Up / Down
SPACE         -> Single Shot
E             -> Spread Shot
D             -> Wide Shot
Q             -> Ultimate Blast

--------------------------------------------------------------------------
[ ADMIN SETUP: URL INJECTION ]
--------------------------------------------------------------------------

[ 1. GLOBAL SETTINGS ]
-------------------------------------------------------------------------
?espeed=1.0   -> Multiplier for all enemy speeds (e.g., 2.0 is double speed).
?burst=3      -> How many bullets are fired in a single "Burst" command.
?spawn=60     -> Frames between enemy spawns. (Lower = More Dense/Harder).

[ 2. PLAYER PARAMETERS ]
-------------------------------------------------------------------------
?channel=NAME  -> Connects to a specific Twitch user.
?ship=URL      -> Replaces the ship with a custom PNG link.
?emote=URL     -> Injects an emote into the ship's cockpit.
?emoteX=0.5    -> Horizontal position (0.0 to 1.0).
?emoteY=0.5    -> Vertical position (0.0 to 1.0).

[ 3. ENEMY PARAMETERS ]
-------------------------------------------------------------------------
Target specific enemies by ID (1-5). Example: e1, e2, etc.

?e1=URL        -> Replaces the image for Enemy 1.
?e1_emote=URL  -> Replaces the emote for Enemy 1.
?e1_ex=0.5     -> Horizontal position of Enemy 1 emote (0.0 to 1.0).
?e1_ey=0.5     -> Vertical position of Enemy 1 emote (0.0 to 1.0).

--------------------------------------------------------------------------
[ IMPORTANT NOTES ]
--------------------------------------------------------------------------
* FALLBACKS: If you leave a parameter out, the game uses built-in defaults.
* SPAWN DENSITY: To make the game harder, decrease the "?spawn" number.
* IMAGE REQUIREMENTS: Ship PNG should have transparency for the cockpit.
* ASSETS: Ensure all local .png files are in the same folder as the HTML.

==========================================================================
