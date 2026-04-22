 =========================================================================
                   VRM AI CHATBOT (OBS TRANSPARENT EDITION)
==========================================================================

[ DESCRIPTION ]
An interactive, 3D VRM avatar designed for Twitch streamers. The avatar 
listens to chat, thinks using AI, and responds with animated speech 
bubbles. Features an advanced priority-based state system to ensure 
proactive conversation and a dedicated Developer Test Tool for easy 
asset management. Designed for seamless OBS integration.
--------------------------------------------------------------------------
[ FILE NAME NOTE ]
---------------------------------------------------------------------------
File names are case-sensitive for example if you type "AvtarMove sad" it 
will not work, use instead "AvtarMove Sad"  

--------------------------------------------------------------------------
[ QUICK START ]
---------------------------------------------------------------------------
1. Place your .vrm model in the /VRM/ folder.
2. Place your .vrma animations in the /VRMA/ folder.
3. Update your animation list in vrma.ini (Case-sensitive).
3. Open the HTML file via a local web server (Live Server, XAMPP, etc.).
4. Add as a "Browser Source" in OBS with "Allow Transparency" checked.
5. Chat.ini holds all the questions that you would like the ChatBot to use.

--------------------------------------------------------------------------
[ DEBUGGING & TESTING ]
---------------------------------------------------------------------------
DEVELOPER TEST TOOL (test_animations.html)
https://mohtecgames.github.io/TwitchGames/ChatBotVRM/Ai-TestAnimV1.htm

The Test Tool is highly recommended for setup. It includes:
- ANIMATION DROPDOWN: Automatically loads all animations from your vrma.ini.
- DURATION READOUT: Instantly shows the duration (in seconds) defined in .ini.
- AVATAR LOADER: Type a filename to test different models instantly.
- STATE MONITOR: Watch the HUD to see if the bot is IDLE, THINKING, or TALKING.

--------------------------------------------------------------------------
[ CHAT GUIDE - VIEWERS ]
--------------------------------------------------------------------------
[Trigger] [Message] -> Asks the AI a question.
Example: "AI, tell me a joke!" 
(Note: "AI" is the default trigger word. If your avatar is named "Luna", 
you must type "Luna, tell me a joke!")

--------------------------------------------------------------------------
[ ADMIN SETUP: URL INJECTION ]
--------------------------------------------------------------------------
All settings are controlled via URL parameters for instant reconfiguration.

[ 1. IDENTITY & TWITCH ]
-------------------------------------------------------------------------
?avatar=NAME   -> Sets the AI's name and the required Chat Trigger word.
?channel=NAME  -> The Twitch channel the bot will monitor.

[ 2. AI ENGINE SETTINGS ]
-------------------------------------------------------------------------
?api_type=TYPE -> Select engine: 'google' (Default), 'local', 'remote'
?model=NAME    -> The specific AI model ID (e.g., gemma3n:e2b).
?ctx=12000     -> The context window size (memory) for the AI.

[ 3. CONNECTION SETTINGS ]
-------------------------------------------------------------------------
?url=URL       -> (Local/Remote) The endpoint for your API (e.g., 192.168.1.5:11434).
?key=YOUR_KEY  -> (Google Mode) Your Gemini API Key.

--------------------------------------------------------------------------
[ IMPORTANT NOTES ]
--------------------------------------------------------------------------
* MIXED CONTENT WARNING (CRITICAL): If you host this on GitHub Pages 
  (HTTPS), your remote API URL MUST also use HTTPS. Browsers will 
  BLOCK any connection from an HTTPS site to an HTTP address. 
  (Exception: 'localhost' or '127.0.0.1' is always allowed).

* PRIORITY STATE LOGIC: The bot uses a priority system. Proactive 
  conversations (the 40-second timer) will now correctly interrupt 
  idle animations, ensuring the bot doesn't "dance through" its 
  scheduled speaking time.

* ERROR RESILIENCE: The bot is designed to not "lock up" on network 
  failures. If a connection attempt fails (e.g., a timeout), the 
  cooldown is bypassed so the bot can attempt to reconnect immediately.

* OBS TRANSPARENCY: Ensure "Allow Transparency" is ENABLED in the OBS 
  Browser Source properties.

* ASSET PATHS: Ensure your folders are named exactly /VRM/ and /VRMA/ 
  relative to the HTML file.

==========================================================================
