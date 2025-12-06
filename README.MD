# EchoStory · Blueprint of a Quiet Revolution

## Why This Exists

This work is a nervous system journey you can listen to.

It teaches your body the difference between reaction, regulation, and relationship design.

It's not music for entertainment — it's architecture for the way you love.

---

## Who It's For

✔️ People who sabotage connection without wanting to  
✔️ Couples moving from trauma-bond to intentional love  
✔️ Therapists & coaches using narrative somatics

This reframes the project as a tool, not a playlist.

---

## The Journey

A three-chamber EchoStory experience built around the Responce trilogy:

1. **My Chaos Ain't Your Crisis** — When love stops feeling like a threat
2. **I Don't Hear Danger In Your Voice** — The moment calm doesn't feel like a trap
3. **We Don't Flinch We Build** — Co-designing the future, love as architecture instead of emergency

The HTML player page stitches these tracks into a single narrative arc:  
**Trauma → Safety → Architecture** — **Reaction → Regulation → Relationship Design**.

---

## Files in This Folder

Core audio:

- `my-chaos-ain't-your-crisis.mp3`
- `i-don't-hear-danger-in-your-voice.mp3`
- `we-don't-flinch-we-build.mp3`

Alt mixes (for future swaps / alternate cuts):

- `my-chaos-ain't-your-crisis-alt.mp3`
- `i-don't-hear-danger-in-your-voice-alt.mp3`
- `we-don't-flinch-we-build-alt.mp3`

Text:

- `lyrics.txt` – raw/combined lyrics source.
- `echo-story-blueprint.html` – **EchoStory player page** (name it whatever you prefer).

> ✅ The HTML player expects the *non-alt* `.mp3` filenames above by default.

If you change file names or move audio into subfolders, you’ll need to update the `<audio src="...">` paths inside the HTML.

---

## What the HTML Player Does

The EchoStory page is a **self-contained, dark-theme story console** that provides:

### 1. Global "EchoStory Flow" Mode
- A **3-step audio sequence**:
  1. `my-chaos-ain't-your-crisis.mp3`
  2. `i-don't-hear-danger-in-your-voice.mp3`
  3. `we-don't-flinch-we-build.mp3`
- Clicking **“Play EchoStory Flow”**:
  - Starts at Chamber I and automatically chains to II and III.
  - Scrolls the page to the current chamber as each track starts.

### 2. Per-Chamber Sections

Each chamber in the HTML page includes:

- **Story header**: Chamber number, song title, tagline/theme.
- **Track player card**:
  - Short description of what this track represents in the narrative.
  - Audio controls for that specific song.
- **Spoken EchoStory script**:
  - Narrative paragraphs written to be read or performed over/around the track.
- **Full lyrics**:
  - Lyrics rendered inside a `<details>` / `<summary>` collapsible block for each song.

Chambers:

1. **Chamber I – My Chaos Ain’t Your Crisis**
   - Theme: naming the pattern, taking ownership of reactions.
2. **Chamber II – I Don’t Hear Danger In Your Voice**
   - Theme: nervous system learning it’s finally safe.
3. **Chamber III – We Don’t Flinch We Build**
   - Theme: co-designing the future, love as architecture instead of emergency.

---

## How to Use (Local Playback)

### 1. Windows (local file)

1. Make sure this folder contains:
   - `echo-story-blueprint.html`
   - All three `.mp3` files (non-alt versions) with the exact names listed above.
2. Double-click `echo-story-blueprint.html` to open in your default browser.
3. Use:
   - **Play EchoStory Flow** for the full narrative.
   - Individual chamber players to jump to specific songs.
   - Timeline on the right to navigate between chambers.
   - **All Lyrics** button to jump to the final lyrics block.

If the audio doesn’t play, check:

- Browser security around local file audio (Chrome/Edge usually fine).
- That the `.mp3` filenames match exactly (smart quotes, spaces, etc).

---

## Customization Notes

### Swap to Alt Mixes

If you want the page to use the `.alt` versions:

1. Open `echo-story-blueprint.html` in a code editor.
2. Find the `<audio>` tags and update `src` attributes, for example:

```html
<audio id="audioChaosV2" src="my-chaos-ain't-your-crisis-alt.mp3" preload="metadata"></audio>
