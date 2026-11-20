# CyberClipping — by Cyberzone

Link paste karo, captioned 9:16 clips lo — about 2 minutes mein. Free, local, open-source.
YouTube / Twitch / Kick link ya apni MP4 se vertical clips (Reels / Shorts / TikTok).

> **Credit:** Ye tool [NeonClipping](https://github.com/iamajmeena/neonclipping)
> by Ajay K Meena par based hai, MIT License ke under.
> Original code aur idea un ka hai — ye sirf Cyberzone branding
> wala copy hai, naya invention nahi. LICENSE file mein original
> copyright waise ka waisa rakha gaya hai.

## Repo (jab live ho)

- **Cyberzone copy:** https://github.com/Cyberzone-pk/cyberclipping
- **Original (upstream):** https://github.com/iamajmeena/neonclipping

## Install (Windows — sab se easy)

1. `CyberClipping-Setup.bat` download kar ke double-click karo
   (Releases page se). Ye Python + FFmpeg check karega, app install
   karega, Desktop shortcut banayega aur app khol dega.
2. Ya manual:
   ```bash
   git clone https://github.com/Cyberzone-pk/cyberclipping
   cd cyberclipping
   ./run.ps1        # Windows
   ./run.sh         # Linux / macOS
   ```
3. Chrome mein kholo: http://127.0.0.1:8770

Requirements: Python 3.10+, FFmpeg. Optional: Ollama + `ollama pull llama3.2:3b`
(AI titles/hooks ke liye), NVIDIA GPU (fast transcription ke liye).

## Use karo — 4 steps

1. YouTube / Twitch / Kick link paste karo, ya MP4 upload karo.
2. Facecam position chuno (top-left, top-right, bottom-left,
   bottom-right, bottom-centre, ya none) — ya Step 03 mein
   facecam aur gameplay boxes khud draw karo.
3. **Make clips** dabao.
4. Clips ek-ek kar ke aati hain — preview dekho, **Download MP4** dabao.
   Sab clips **My clips** mein bhi rehti hain.

## Settings

- **Mode:** Fast (default, ~2 min) ya Deep (slow, zyada smart)
- **Clips:** 1–12
- **Min / Max length:** jaise 30–60 ya 30–80 seconds
- **Caption style:** GTA Neon, Hormozi, MrBeast, Impact, Clean
- **Caption language:** Auto (Hindi → Hinglish), Hinglish, Hindi, English
- **Caption accuracy:** Accurate (default), Fast, Best Hindi

## Branding is mein kya change hai

- Naam: NeonClipping → **CyberClipping**
- Repo: `iamajmeena/neonclipping` → `Cyberzone-pk/cyberclipping`
- Theme: Cyberzone navy (`#060d18`) + cyan-blue (`#00b4ff`)
- Sidebar/footer: **BY CYBERZONE • CYBERZONE.PK**
- Donate / Razorpay links hata diye gaye hain (button hidden hai)
- Env vars: `NEONCLIPPING_*` → `CYBERCLIPPING_*`
  (jaise `CYBERCLIPPING_PORT=8771`, `CYBERCLIPPING_CPU=1`)
- Port wahi: **8770**

## Honest limits

- Highlight picking heuristic + chhota local LLM hai — loud,
  energetic, quotable moments dhoondhta hai, guaranteed viral nahi.
  Post karne se pehle clip dekh lo.
- YouTube captions na hon (Twitch VOD, MP4) to local speech model
  slow ho sakta hai, captions rough ho sakte hain.
- Koi account, subscription ya upload nahi — sab kuch aapke
  computer par chalta hai (`127.0.0.1` only).
