===========================================================
===           TWITCH MYSTICAL TAROT (ULTIMATE)          ===
===========================================================

[ VIEWER GUIDE (Twitch Chat) ]
Type these commands to receive a mystical reading:
tarotdeck [your question]  -> General reading
tarotbeginnings            -> Focus on new starts
tarotcareer                -> Focus on work/ambition
tarotmoney                 -> Focus on finances
tarotlove                  -> Focus on romance/relationships
tarotfriendsfamily         -> Focus on social connections
tarothealth                -> Focus on wellness/vitality
tarothigherguidance        -> Focus on spiritual direction

 
[ EASY CONFIGURATION ]
Instead of manually typing long URLs, use the provided URL Maker tool:

URL Maker: 
https://mohtecgames.github.io/TwitchGames/TarotTwitch/TarotV1.6 URLMaker.HTML
 
[ STREAMER GUIDE (Manual Controls) ]
Use the on-screen buttons for testing and management:
TEST READING               -> Manually triggers a reading (for testing)
Reset Timer (20M)          -> Resets the global cooldown to default
10s Timer                  -> Sets a quick 10-second cooldown for testing

[ ADMIN SETUP: URL INJECTION ]
You can fully customize the tarot experience without touching 
the code by adding "Parameters" to the end of your URL.

PARAMETER LIST:
-------------------------------------------------------
?TWITCH_CHANNEL=NAME        -> Connects to a specific Twitch user.
?COOLDOWN_SECONDS=SEC       -> Global cooldown between readings (seconds).
?USER_COOLDOWN_SECONDS=SEC  -> Cooldown per individual user (seconds).
?READING_DURATION_MS=MS     -> How long the reading stays visible (ms).
?CARD_FLIP_DELAY_MS=MS      -> Delay between individual card flips (ms).
?READ_FLIP_DELAY_MS=MS      -> Delay before the text reading appears (ms).
?STATUS_TEXT_PRIMARY=TEXT   -> The main top line of the status bar.
?STATUS_TEXT_COMMANDS=TEXT  -> The bottom line of the status bar.

[ EXAMPLES OF USE ]
---------------------------------------------------------
1. THE "DEFAULT" MODE (No injection):
   index.html
   (Uses: MohTecGames, 20M Cooldown, Default Status Text)

2. THE "CUSTOM CHANNEL" MODE:
   index.html?TWITCH_CHANNEL=YourTwitchName

3. THE "FAST-PACED" MODE (Short cooldowns & fast flips):
   index.html?COOLDOWN_SECONDS=60&CARD_FLIP_DELAY_MS=500&READ_FLIP_DELAY_MS=5000

4. THE "FULLY BRANDED" MODE (Custom text & long reading):
   index.html?TWITCH_CHANNEL=Name&STATUS_TEXT_PRIMARY=Ask%20the%20Cards!&READING_DURATION_MS=45000

[ IMPORTANT NOTES ]
---------------------------------------------------------
* FALLBACKS: If you leave a parameter out, the script 
  automatically uses the built-in default values.
* URL ENCODING: When injecting text (like STATUS_TEXT), 
  you MUST use URL encoding for spaces and symbols.
  (Example: "Ask the Cards" -> "Ask%20the%20Cards")
* HTML INJECTION: You can include <br> or <small> tags 
  in your text parameters to format the status bar.
* ASSETS: Ensure all card images are located in the 
  "Cards/" folder relative to this HTML file.

===========================================================
