# MohTecGames Interactive Suite

A collection of high-performance, web-based interactive experiences. This suite includes a classic arcade game for local play and two specialized interactive applications designed specifically for **Twitch Streamers** to engage their live audiences via chat integration.

---

## 🎮 Games Overview
https://mohtecgames.github.io/TwitchGames/
### 1. Flappy Bird Fullscreen Pro
A polished, responsive, and fullscreen implementation of the classic arcade sensation. This version is optimized for both desktop and mobile browsers, featuring smooth physics and a parallax-style background.

*   **Genre:** Arcade / Casual
*   **Key Features:** 
    *   Responsive design (scales to any screen size).
    *   High-score tracking via `localStorage`.
    *   Smooth gravity and collision physics.
*   **Controls:**
    *   **Desktop:** `Spacebar` or `Arrow Up` to flap.
    *   **Mobile/Touch:** Tap the screen to flap.

### 2. Twitch Space Shooter Pro (Parametric Burst)
An action-packed space shooter where the **Twitch Chat is the controller**. This game uses `ComfyJS` to bridge the gap between the streamer's audience and the game engine, allowing viewers to pilot the ship and trigger massive attacks.

*   **Genre:** Twitch-Integrated Arcade Shooter
*   **Key Features:**
    *   **Chat-Driven Gameplay:** Viewers control movement and combat via chat commands.
    *   **Parametric Burst System:** Multiple firing modes including spread shots and "Ultimate" bursts.
    *   **Dynamic Enemy AI:** Enemies feature different behaviors (Linear, Wander, and Zigzag).
    *   **Visual Effects:** Particle explosions and starfield parallax.
*   **Twitch Chat Commands:**
    *   `gamestart`: Resets and starts a new game.
    *   `u`: Move ship **Up**.
    *   `d`: Move ship **Down**.
    *   `s1`: Trigger **Standard Shot**.
    *   `s2`: Trigger **Burst Shot**.
    *   `s3`: Trigger **Spread Shot**.
    *   `ult`: Trigger **Ultimate Burst** (60s Cooldown).

### 3. Twitch Mystical Tarot
A mystical, interactive experience designed for streamers to provide live "readings" to their community. The game interprets viewer questions and generates a three-card spread (Past, Present, and Future) with narrative insights.

*   **Genre:** Interactive Utility / Community Engagement
*   **Key Features:**
    *   **Automated Narratives:** Generates cohesive readings based on card meanings.
    *   **Topic-Specific Insights:** Readings can be tailored to specific life categories (Love, Career, etc.).
    *   **Cinematic Animations:** Smooth 3D card-flip transitions and overlay text.
    *   **Cooldown Management:** Prevents spam by managing user and global cooldowns.
*   **Twitch Chat Commands:**
    *   **To start a reading:** Type `tarotdeck` followed by your question.
    *   **To specify a category:**
        *   `tarotbeginnings` (New starts)
        *   `tarotcareer` (Work/Ambition)
        *   `tarotmoney` (Finances)
        *   `tarotlove` (Relationships)
        *   `tarotfriendsfamily` (Social circles)
        *   `tarothealth` (Wellness)
        *   `tarothigherguidance` (Spiritual/Universe)

---

## 🛠️ Technical Stack

*   **Core:** HTML5, CSS3, JavaScript (ES6+).
*   **Rendering:** HTML5 Canvas API for high-performance 2D graphics.
*   **Twitch Integration:** [ComfyJS](https://github.com/instafluff/comfy.js) for real-time chat parsing and EventSub support.
*   **Storage:** `localStorage` for persistent high-score tracking.

---

## 📜 Copyright & Attribution

**CREATED BY:** MohTecGames

**NOTICE:** This work is protected. Any reproduction, distribution, or use of this code, its logic, or its assets requires prior written approval from **MohTecGames**.

**CREDITS:**
*   **Tarot Meanings:** Inspired by *"The Big Book of Tarot Meanings"* by Sam Magdaleno.
*   **Twitch Integration:** Utilizes Comfy.JS by Instafluff.
