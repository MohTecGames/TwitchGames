Here is your updated `README.md`. I have integrated the **VRM AI Chatbot** as the fourth major experience and added a dedicated **Credits** section to include the avatar sources and the technical conversion tool.

***

# MohTecGames Interactive Suite

A collection of high-performance, web-based interactive experiences. This suite includes classic arcade games, specialized interactive applications for Twitch streamers, and an advanced AI-driven 3D companion designed to engage live audiences via chat integration.

## 🎮 Games Overview

[https://mohtecgames.github.io/TwitchGames/](https://mohtecgames.github.io/TwitchGames/)

### 1. Flappy Bird Fullscreen Pro
A polished, responsive, and fullscreen implementation of the classic arcade sensation. This version is optimized for both desktop and mobile browsers, featuring smooth physics and a parallax-style background.

*   **Genre:** Arcade / Casual
*   **Key Features:**
    *   Responsive design (scales to any screen size).
    *   High-score tracking via `localStorage`.
    *   Smooth gravity and collision physics.
*   **Controls:**
    *   **Desktop:** Spacebar or Arrow Up to flap.
    *   **Mobile/Touch:** Tap the screen to flap.

---

### 2. Twitch Space Shooter Pro (Parametric Burst)
An action-packed space shooter where the Twitch Chat is the controller. This game uses ComfyJS to bridge the gap between the streamer's audience and the game engine, allowing viewers to pilot the ship and trigger massive attacks.

*   **Genre:** Twitch-Integrated Arcade Shooter
*   **Key Features:**
    *   **Chat-Driven Gameplay:** Viewers control movement and combat via chat commands.
    *   **Parametric Burst System:** Multiple firing modes including spread shots and "Ultimate" bursts.
    *   **Dynamic Enemy AI:** Enemies feature different behaviors (Linear, Wander, and Zigzag).
    *   **Visual Effects:** Particle explosions and starfield parallax.
*   **Twitch Chat Commands:**
    *   `gamestart`: Resets and starts a new game.
    *   `u`: Move ship Up.
    *   `d`: Move ship Down.
    *   `s1`: Trigger Standard Shot.
    *   `s2`: Trigger Burst Shot.
    *   `s3`: Trigger Spread Shot.
    *   `ult`: Trigger Ultimate Burst (60s Cooldown).

---

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

### 4. VRM AI Chatbot (Pro Edition)
An advanced, interactive 3D companion designed to live directly on your stream. This companion uses Large Language Models (LLMs) to listen to your Twitch chat and respond in real-time with animated speech bubbles.

*   **Genre:** AI-Driven Interactive Avatar
*   **Key Features:**
    *   **Multi-Engine AI Support:** Connect via Google Gemini, Local Ollama, or a Remote API.
    *   **3D Immersion:** Fully animated VRM model integration with dynamic facial/body expressions.
    *   **Streamer Optimized:** Built-in transparency support for seamless OBS integration.
    *   **Intelligent Constraints:** Hardcoded prompt reinforcement ensures the AI keeps replies concise and chat-friendly.
*   **Twitch Chat Commands:**
    *   `[Trigger] [Message]`: Asks the AI a question.
    *   *Example:* `AI, tell me a joke!` (Note: Trigger word depends on your avatar's name).

---

## 🛠️ Technical Stack

*   **Core:** HTML5, CSS3, JavaScript (ES6+).
*   **Rendering:** HTML5 Canvas API for high-performance 2D graphics; Three.js & WebGL for 3D VRM rendering.
*   **Twitch Integration:** ComfyJS for real-time chat parsing and EventSub support.
*   **Storage:** `localStorage` for persistent high-score tracking.

---

## 📜 Copyright & Attribution

**CREATED BY: MohTecGames**

**NOTICE:** This work is protected. Any reproduction, distribution, or use of this code, its logic, or its assets requires prior written approval from MohTecGames.

**CREDITS:**

*   **Avatars & Animations:** 3D Models and VRM animations provided by [OpenSourceAvatars.com](https://opensourceavatars.com).
*   **Technical Tools:** Special thanks to the [fbx2vrma-converter](https://github.com/tk256ailab/fbx2vrma-converter) for providing the essential tools for seamless animation conversion.
*   **Twitch Integration:** Utilizes Comfy.JS by Instafluff.
*   **Tarot Meanings:** Inspired by "The Big Book of Tarot Meanings" by Sam Magdaleno.
