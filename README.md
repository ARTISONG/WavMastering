# 🎚️ AI Audio Mastering Studio

เว็บแอปมาสเตอร์เพลงอัตโนมัติ ทำงานในเบราว์เซอร์ 100% (ไฟล์เพลงไม่ถูกอัปโหลดไปเซิร์ฟเวอร์)
รองรับ WAV / MP3 / FLAC / AIFF / M4A — ปรับแต่งผ่าน slider พร้อมฟังตัวอย่างสด

## ฟีเจอร์
- **Pre-Master Analysis** — LUFS (BS.1770), True Peak, Headroom, Dynamic Range, Stereo, Noise, DC offset, Clipping
- **AI One-Click / Auto ต่อโมดูล** — วิเคราะห์เพลงแล้วตั้งค่าให้อัตโนมัติ (กด ⚡ Auto แยกแต่ละโมดูลได้)
- **Mastering Chain** — EQ, Dynamic EQ, Multiband Compressor, Glue, Saturation, Exciter, De-Esser, Harmonic Enhancer, Stereo Imaging, True-Peak Limiter (เปิด/ปิดแยกได้)
- **Loudness Target** — Spotify / Apple / YouTube / TIDAL / Broadcast / Podcast / Custom
- **Preset & AI Character** — 19 Preset + 10 Character
- **Fade / Silence Trim / Auto Repair**
- **Quality Check** — PASS / WARNING / FAIL พร้อมคำแนะนำวิธีแก้
- **Export** — WAV (16/24/32-bit), MP3 (320/256/192) + Dither + resample
- **Batch / Album Master** — normalize ทั้งอัลบั้มให้สมดุล หรือทุกเพลงเท่ากัน → ZIP

## ใช้งาน
เปิด `index.html` ในเบราว์เซอร์ (Chrome/Edge/Safari) ได้เลย — หรือดูเวอร์ชันออนไลน์ผ่าน GitHub Pages

## เทคนิค
- Web Audio API + ScriptProcessor DSP (ทำงานได้ทั้ง `file://` และผ่านเซิร์ฟเวอร์)
- Integrated LUFS มาตรฐาน ITU-R BS.1770 (K-weighting + gating)
- ใช้ CDN: [lamejs](https://github.com/zhuker/lamejs) (MP3), [JSZip](https://stuk.github.io/jszip/) (batch ZIP)

## Deploy
Push ขึ้น branch `main` แล้ว GitHub Actions จะ deploy ขึ้น GitHub Pages อัตโนมัติ
(ต้องเปิด Settings → Pages → Source = **GitHub Actions** ครั้งแรก)
