# Waktu Solat OBS · MKSLB

Browser source OBS (1920×1080) untuk live stream Masjid Kampung Sungai Lang Baru:
waktu solat seterusnya, countdown 3 bulatan, dan jalur 8 waktu.

Data dari [API waktu solat](https://apiwaktusolatsgr03.vercel.app/api/waktu-solat)
(2026: JAKIM e-Solat · 2027: Takwim Mufti Selangor, Daerah Kuala Langat).

## Pasang dalam OBS
1. Sources → **+** → **Browser**
2. **Local file** → pilih `index.html` (atau URL hosting jika diletak di Vercel)
3. Width **1920**, Height **1080**

## Nota
- Perlu internet (tarik data dari API); auto-segar setiap hari baru.
- `adjust=jugra` hanya berkesan untuk 2026. Untuk 2027, API ikut takwim daerah (tiada pelarasan Jugra).
- Nak jadikan overlay atas kamera: tukar `background:var(--green-800)` pada `html,body` kepada `background:transparent`.
