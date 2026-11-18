# roblox-cloud-pc

Cloud PC sekali pakai buat publish game Roblox "Slurp a Brainrot" (roblox-brainrot-01)
dari HP — akun GitHub ini akun buangan khusus buat ini, bukan akun utama.

Cara pakai (Jumat 20 Nov, akun Roblox sandi26_id baru bisa publish mulai hari itu):
1. Di aplikasi GitHub / github.com: repo ini > Actions > `roblox-studio-rdp` > Run workflow.
2. Tunggu job jalan, buka log-nya, catat RUSTDESK ID + PASSWORD yang muncul di log.
3. Di HP: buka aplikasi RustDesk, masukkan ID + password, konek ke PC cloud.
4. Di PC cloud: buka `game.rbxl` di Roblox Studio, File > Publish to Roblox As >
   buat experience baru "Slurp a Brainrot", deskripsi wajib berisi kode
   `makefun-palm-mesa-ginger`, audience Public, upload thumbnail pertama.
5. Kirim link play + universe id + place id ke Muse, lalu matikan job-nya
   (Cancel workflow) — PC-nya langsung hancur.

File di repo ini:
- `game.rbxl.b64` — game final (base64; workflow decode jadi game.rbxl di runner)
- `.github/workflows/rdp.yml` — workflow-nya (install RustDesk 1.5.3 + Roblox Studio)
- Jangan taruh password / token apa pun di repo ini.
