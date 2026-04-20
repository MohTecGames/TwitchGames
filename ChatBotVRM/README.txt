=========================================================================
                   VRM AI CHATBOT (OBS TRANSPARENT EDITION)
==========================================================================

[ DESCRIPTION ]
An interactive, 3D VRM avatar designed for Twitch streamers. The avatar 
listens to chat, thinks using AI, and responds with animated speech 
bubbles. Designed with a transparent background for seamless OBS 
integration.

--------------------------------------------------------------------------
[ QUICK START ]
---------------------------------------------------------------------------
1. Place your .vrm model in the /VRM/ folder.
2. Place your .vrma animations in the /VRMA/ folder.
3. Open the HTML file via a local web server (Live Server, XAMPP, etc.).
4. Add as a "Browser Source" in OBS with "Allow Transparency" checked.

--------------------------------------------------------------------------
[ DEBUGGING & TESTING ]
---------------------------------------------------------------------------
ANIMATION TEST BENCH (test_animations.html)
If your avatar is not animating correctly, use the Test Bench script. 
It will automatically cycle through every animation in your list to 
verify that all .vrma files are loading and playing without errors.

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
All settings are controlled via URL parameters to allow for instant 
reconfiguration without touching the code.

[ 1. IDENTITY & TWITCH ]
-------------------------------------------------------------------------
?avatar=NAME   -> Sets the AI's name and the required Chat Trigger word.
?channel=NAME  -> The Twitch channel the bot will monitor.

[ 2. AI ENGINE SETTINGS ]
-------------------------------------------------------------------------
?api_type=TYPE -> Select engine: 'google' (Default), 'local', 'server', 'online'
?model=NAME    -> The specific AI model to use (e.g., llama3.2:3b).
?ctx=12000     -> The context window size (memory) for the AI.

[ 3. CONNECTION SETTINGS ]
-------------------------------------------------------------------------
?url=URL       -> (Local Mode) The endpoint for your Ollama API.
?server_url=U  -> (Server Mode) Your custom backend API URL.
?online_url=U  -> (Online Mode) Your external API endpoint.
?online_key=K  -> (Online Mode) Your API Bearer Token/Key.

--------------------------------------------------------------------------
[ IMPORTANT NOTES ]
--------------------------------------------------------------------------
* OBS TRANSPARENCY: Ensure "Allow Transparency" is ENABLED in the OBS 
  Browser Source properties, or the background will appear black.
* AI LIMITS: The system is hardcoded to force the AI to keep replies 
  under 40 words to ensure fast, readable chat interaction.
* ASSET PATHS: Ensure your folders are named exactly /VRM/ and /VRMA/ 
  relative to the HTML file.
* GOOGLE API: To use the default Google mode, you must insert your 
  Gemini API key directly into the script's GOOGLE_KEY variable.

==========================================================================
