===================================================
===       TWITCH SPACE SHOOTER PRO (ULTIMATE)   ===
===================================================
 
[ PLAYER GUIDE (Twitch Chat) ]
Type these commands to help the pilot:
u / d         -> Move Ship UP / DOWN
s1 / s2 / s3  -> SHOOT (Single / Spread / Wide)
ult           -> ULTIMATE BLAST (60s Cooldown)
gamestart     -> Restart Game

[ STREAMER GUIDE (Keyboard) ]
Play manually using these keys:
W / S         -> Move Up / Down
SPACE         -> Single Shot
E             -> Spread Shot
D             -> Wide Shot
Q             -> Ultimate Blast

[ ADMIN SETUP: URL INJECTION ]
You can fully customize the game without touching the code 
by adding "Parameters" to the end of your URL.

PARAMETER LIST:
---------------------------------------------------
?channel=NAME  -> Connects to a specific Twitch user.
?ship=URL      -> Replaces the ship with a custom PNG link.
?emote=URL     -> Injects an emote into the ship's cockpit.
?emoteX=0.0    -> Horizontal position of emote (0.0 = Left, 0.5 = Center, 1.0 = Right).
?emoteY=0.0    -> Vertical position of emote (0.0 = Top, 0.5 = Middle, 1.0 = Bottom).

[ EXAMPLES OF USE ]
---------------------------------------------------
1. THE "DEFAULT" MODE (No injection):
   index.html
   (Uses: MohTecGames, ShipHero.png, No Emote)

2. THE "EMOTE ONLY" MODE (Using default ship):
   index.html?channel=yourname&emote=https://link.com/emote.png

3. THE "FULL CUSTOM" MODE (Custom Ship + Emote + Position):
   index.html?channel=yourname&ship=https://link.com/ship.png&emote=https://link.com/emote.png&emoteX=0.5&emoteY=0.2

[ IMPORTANT NOTES ]
---------------------------------------------------
* FALLBACKS: If you leave a parameter out, the game 
  automatically uses the built-in defaults.
* EMOTE POSITION: Use decimals (like 0.5) for X and Y. 
  These are relative to the ship's size.
* IMAGE REQUIREMENTS: For the "Cockpit" effect, your 
  Ship PNG should have a transparent area where 
  the pilot sits.
* ASSETS: Ensure all local .png files (Enemy1, etc.) 
  are in the same folder as the HTML file.

===================================================
