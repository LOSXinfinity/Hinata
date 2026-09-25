# Hinata · 片想いの連鎖

> *The Chain of Unrequited Love*

A scroll-native interactive poem in three movements. Built for the browser as a single self-contained HTML file — no build step, no dependencies, no framework. Just vanilla JS, CSS custom properties, and 70 hand-crafted frames.

---

## The Experience

### I. The Lantern (Finale)
Three figures under one lantern. Naruto is always lit.  
Move your cursor — decide who stands beside him in the light:  
**Sakura**, laughing at his jokes — or **Hinata**, sitting apart so no one asks.

The light has inertia. It drifts when you let go.  
A ghost trail follows. Grain and bloom breathe on the frame.

> 「ナルトくん…」 — *Hinata's whisper*  
> 「サクラちゃん！」 — *Naruto's shout*

### II. The Swing
The academy swing. Naruto alone. Everyone else collected by somebody.  
Hinata watches from the shadows — *watching him be lonely felt closer than being seen by him.*

Parallax layers drift at different speeds. The type moves furthest.  
Depth born from the gap between speeds.

### III. The Film (Under the Tree)
Seventy stills from one evening. Scroll to play it through.  
Cross-dissolved frames. Pointer parallax with a gentle lag.  
Vertical captions appear at precise moments — each a haiku of what goes unsaid.

> 見つめる — *She has been standing there a while. Her heart is already saying his name.*  
> 気づかない — *He never turns around. Not once.*  
> 恋の目 — *Because his eyes are already full of someone else entirely.*  
> そして — *And she is thinking about a boy who is not thinking about her.*

---

## The Philosophy

**Kataomoi (片想い)** — one-sided love. Not tragic. Not lacking.  
A love that *chooses* to remain unspoken. That finds completeness in witnessing.  
That sits on the swing beside the empty seat and calls it closeness.

This piece does not resolve. It *lingers*.  
The lantern never lights both. The swing never fills. The tree never witnesses a confession.  
And that is exactly the point.

> *To love someone is to illuminate them.*  
> *To love someone who loves another is to hold the lantern for the both of them —*  
> *and stand in your own light.*

---

## Technical Notes

- **Single file**: `index.html` — open directly in any modern browser
- **Assets**: 70 WebP frames (`frames/f001.webp` … `f070.webp`) + `swing.webp` + `trio.webp`
- **Fonts**: Google Fonts (Yuji Syuku, Zen Kaku Gothic New, Zen Maru Gothic)
- **Respects** `prefers-reduced-motion` and `hover: none`
- **No cursor on touch** — petals and lantern drift on their own
- **IntersectionObserver** gates the heavy lantern canvas to when it's on screen
- **DPR-clamped** canvases (max 2× film, 1.5× lantern) for performance

### Color Tokens (CSS Custom Properties)
```css
--ink:       #000000;   /* pure black ground */
--sumi:      #121016;   /* sumi-e ink wash */
--paper:     #EFE8EA;   /* aged washi */
--mist:      #9A8F9E;   /* morning mist */
--faint:     #4A4351;   /* distant memory */

--hinata:    #9AA4E4;   /* lavender — her chakra, her eyes */
--naruto:    #F59436;   /* orange — his jump suit, his sun */
--sakura:    #F49BBD;   /* cherry blossom — her namesake */
--dusk:      #E8A24C;   /* the swing scene's low sun */
--leaf:      #4E7A45;   /* konoha green */
```

---

## Running Locally

```bash
# No install needed — just serve the folder
npx serve .
# or
python -m http.server 8080
# or any static server
```

Then open `http://localhost:8080`

---

## Credits

**Concept, Design, Code** — A love letter to the quiet ones  
**Source Material** — *Naruto* by Masashi Kishimoto  
**Typefaces** — Yuji Syuku (calligraphic display), Zen Kaku Gothic New / Zen Maru Gothic (UI)  
**Images** — AI-generated frames, curated and sequenced by hand

---

## License
 
*If this moves you, pass it to someone who needs to know they're seen in the dark.*

---

<p align="center">
  <em>木ノ葉隠れの里 · 夜</em><br>
  <em>Konohagakure · After Dark</em>
</p>
