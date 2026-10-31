# ✨ A Little Diwali Surprise for You — Mumbai Darshan Gang

A personalized, rich, interactive, and festive Diwali surprise website crafted for Mumbai Darshan Gang.

---

## 🎵 Festive Background Music & Sound Effects

- **Continuous Background Music**: Features the royalty-free Indian classical instrumental track *"Vadodora Chill Mix"* by Kevin MacLeod (featuring Sitar, Bansuri bamboo flute, subtle Tabla percussion, and festive chimes).
  - Continuous playback across all 5 screens without restarting on screen transitions.
  - Smooth fade-in and fade-out on toggle.
  - Built-in volume slider control.
  - Starts OFF by default to respect browser autoplay policies.
  - Music License: Creative Commons By Attribution 4.0 International (`http://creativecommons.org/licenses/by/4.0/`).
- **Independent Tactile Sound Effects (SFX)**: Web Audio API chimes for diya lighting, gift opening, wax seal breaking, and fireworks can be toggled on/off independently without affecting background music.

---

## 🌟 Interactive Experience & Features

1. **Screen 1 — Light the Diya (Welcome & Intro Sequence)**:
   - Starts with fairy lights cascading on one by one and marigold decorations gently fading in.
   - Prominent interactive diya: **"Tap the diya to light up your Diwali surprise."**
   - Tapping ignites a brighter flame, emits a golden light ripple wave across the screen, triggers sparkle bursts, and plays a warm chime.
   - **Easter Egg**: Tapping the diya 4 times rapidly triggers a bonus confetti and sparkle celebration!

2. **Screen 2 — Open a Festive Gift**:
   - Visitors discover an ornate 3D Diwali gift box with golden ribbons and bow: **"There's a little something waiting for you..."**
   - Tapping the gift pops the lid, unties ribbons, and shoots out golden sparkles and flower petals.
   - The message card gracefully rises from inside the gift box with staggered text animations.

3. **Screen 3 — Your Diwali Fortune (Exciting Reveal)**:
   - An ornate golden scroll/chest: **"Reveal My Fortune"** triggers an anticipation rumble, unrolls the scroll, and bursts confetti.
   - **No-Repeat Guarantee**: Fortunes cycle through all 20 unique fortunes before any repeats can occur.
   - Includes a glowing **"✨ Your Diwali Blessing"** badge.
   - Visitors can **"Draw Another Fortune 🎲"** or **"Continue 💫"**.

4. **Screen 4 — Reveal a Heartfelt Message (Royal Letter)**:
   - A sealed royal purple envelope with a festive wax seal: **"Tap the seal to open your letter ✨"**.
   - Tapping breaks the wax seal, flips the envelope flap, releases floating heart particles and marigold petals, and unfolds the college message card.
   - Clicking **"Let's Celebrate Together 🎇"** triggers a radiant golden light sweep transition directly into the finale.

5. **Screen 5 — The Shared Group Finale (Spectacular Celebration)**:
   - Launches multi-position fireworks salvos across the horizon.
   - Dual confetti cannons fire simultaneously from left and right.
   - **Clickable Row of Diyas**: Visitors can tap each diya along the bottom individually to light them up with sparkle chimes.
   - **"Celebrate Again! 🎆"**: Launches new grand fireworks salvos and dual confetti.
   - **Replay ↺** and **Copy Group Link 🔗** with toast notification.

6. **Interactive Extras & Easter Eggs**:
   - **Background Tap Sparkles**: Tapping any empty space on the background creates a sparkling burst at the cursor/finger position with a crystalline bell chime.
   - **Clicking Marigolds in Toran**: Releases a swirling flurry of marigold petals.
   - **Clicking Rangoli Watermark**: Emits starry sparkles.
   - **Secret Blessing Icon (`🎁`)**: Clicking the gift icon in the header reveals a secret college blessing modal.
   - **Built-in Web Audio API**: Completely synthesizer-based ambient Indian tanpura drone and chimes. Starts muted by default with an easy toggle button (`🔇 Sound OFF` / `🔊 Sound ON`).

---

## 📁 Project Structure

```
Diwali website/
├── index.html          # All 5 interactive screens, modals & vector SVG artwork
├── css/
│   └── style.css       # 3D gift box, envelope animations, ripple waves, responsive styling
├── js/
│   ├── friends.js      # List of 12 friends with nicknames and personalized notes
│   ├── fortunes.js     # 20 non-repeating fortunes managed via shuffled deck
│   ├── particles.js    # Canvas golden fireflies, floating marigold petals & heart particles
│   ├── fireworks.js    # Canvas multi-salvo fireworks, dual-cannon confetti & click sparkles
│   ├── audio.js        # Web Audio API tanpura drone, wax seal snap, chimes & flame sounds
│   └── main.js         # Interactive sequences, gift box & envelope controllers, Easter eggs
└── README.md           # Documentation and testing guide
```

---

## 🚀 How to Test Locally

Simply **double-click `index.html`** in File Explorer (or right-click → **Open with** → **Google Chrome / Microsoft Edge / Brave**).

### Testing URL Parameters:
- **Default Experience**: `index.html`
- **Personalized for Friend 1 (Aarav)**: `index.html?friend=friend01`
- **Personalized for Friend 2 (Ananya)**: `index.html?friend=friend02`
- **Any friend from `friend01` to `friend12`**: `index.html?friend=friend05`
- **Direct Group Finale (Screen 5)**: `index.html?view=group`

---

## ✏️ How to Customize

1. **Friend Names & Notes** (`js/friends.js`):
   Edit the names or custom notes in the `FRIENDS_CONFIG` object.
2. **Fortunes** (`js/fortunes.js`):
   Add or modify fortunes in `DIWALI_FORTUNES`.
3. **Core Messages** (`index.html`):
   Edit the text directly inside each screen's container.
