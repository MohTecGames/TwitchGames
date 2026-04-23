============================================================================
                   TWITCH MEDIA OVERLAY
==========================================================================

[ DESCRIPTION ]
A high-performance, customizable media overlay designed for streamers. 
Allows viewers to summon Tenor GIFs and Klipy media (GIF/MP4) with 
seamless audio integration directly onto your stream via Twitch chat.

--------------------------------------------------------------------------
[ URL MAKER ]
--------------------------------------------------------------------------
Instead of manually typing long URLs, use the provided URL Maker tool:

URL Maker: 
[INSERT YOUR URL MAKER LINK HERE]

--------------------------------------------------------------------------
[ CHAT COMMANDS - VIEWERS ]
--------------------------------------------------------------------------
tenor [id]     -> Summon a Tenor GIF.
klipyPlay [id/link]     -> Summon a Klipy GIF/Vid.
 

--------------------------------------------------------------------------
[ ADMIN SETUP: URL PARAMETERS ]
--------------------------------------------------------------------------

[ 1. CONNECTION & PERMISSIONS ]
------------------------------------------------------------------------
?channel=NAME  -> The Twitch channel to listen to.
?perms=VAL     -> Permission level. Supports combinations! 
                 Example: ?perms=mod,vip (Allows Mods AND VIPs).
                 Options: everyone, mod, vip, sub, mod,vip, mod_vip_sub, ini.
?ini_url=URL   -> Path to your Whitelist (.ini) file.
?ban_url=URL   -> Path to your Blacklist (.ini) file.
?klipy_key=Key -> With no API key the script will not work

[ 2. VISUALS & TIMING ]
------------------------------------------------------------------------
?size=VAL      -> Media size as % of screen (e.g., 30).
?duration=MS   -> How long (ms) the media stays on screen.
?u_cd=MS       -> Global Cooldown (ms) between any two summons.
?user_cd=MS    -> User Cooldown (ms) per individual user.

[ 3. DEBUGGING ]
------------------------------------------------------------------------
?debug=true    -> Enables the real-time technical dashboard on screen.

--------------------------------------------------------------------------
[ IMPORTANT NOTES ]
--------------------------------------------------------------------------
* AUDIO: For KlipyVid, you can check "Control audio via OBS" in the 
  Browser Source properties , this can fix volume issues.
* PERMISSIONS: If using "ini" mode, only users in your whitelist can summon.
* COMBINATIONS: You can mix roles in the URL (e.g., ?perms=mod,sub).
* FOLDER SETUP: Ensure your /data/ folder exists for Whitelist/Blacklist.
* AUTOPLAY: Browsers may block audio until you click the overlay once.

==========================================================================
