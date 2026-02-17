## Solo Leveling Inspirasi

Aplikasi Android (Kotlin) dengan backend perhitungan klasik yang akurat, menggabungkan gamifikasi RPG ala manhwa *Solo Leveling* dengan elemen metafisika Tiongkok (Bazi, Zi Wei Dou Shu, Qi Men Dun Jia, Feng Shui, I Ching). Tujuan: Membuat pengguna merasa sebagai Main Character dalam "game hidupnya". Bagi yang tidak percaya, ini hiburan fun; bagi yang percaya, ini pedoman matematis verifiable oleh ahli (psikolog, metafisikawan, atau matematikawan).

App ini mengubah data kelahiran + waktu real-time menjadi sistem status (HP, MP, STR, dll.), quests harian, musuh (clash elemen), weapon/beast, dan timeline prediksi—semua berbasis rumus deterministik tanpa RNG acak.

## Fitur Utama (Berdasarkan Konsep Gabungan)
- **Player Stats**: HP dari vitalitas elemen, LUCK dari bintang baik/buruk, dll. (Rumus normalisasi: 0-100).
- **Quests & Enemies**: Quest counter musuh (misal hindari arah buruk), generated otomatis dari Qi Men/Feng Shui.
- **Timeline Simulator**: Prediksi per jam dengan slider, update real-time.
- **Gamifikasi**: Leveling (Da Yun sebagai level), achievement milestone hidup, AR elements (opsional).
- **Transparansi**: Setiap stat clickable untuk tampilkan rumus/sumber metafisika.
- **Integrasi**: AI personalisasi quests, komunitas guild, safeguards anti-addiction.

## Konsep Pembanding dari AI
Konsep ini dikumpul dari lima AI sebagai benchmark untuk tim pengembang. Setiap konsep fokus pada aspek berbeda, tapi semuanya matematis dan verifiable. File raw tersedia di branch main:
- **[DeepSeek](https://raw.githubusercontent.com/aiksatria/sololeveling/main/deepseek)**: Detail UI/UX RPG (layout panel, enemy list, quests checkbox). Pemetaan langsung metafisika ke game elements.
- **[Gemini](https://raw.githubusercontent.com/aiksatria/sololeveling/main/gemini)**: Arsitektur teknis (Kotlin MVVM, algoritma normalisasi, pseudocode enemy spawn).
- **[ChatGPT](https://raw.githubusercontent.com/aiksatria/sololeveling/main/chatgpt)**: Engine global dengan normalization layer, quest sebagai strategy, visi sebagai life simulator.
- **[Grok](https://raw.githubusercontent.com/aiksatria/sololeveling/main/grok)**: Gamifikasi modern (XP geometris, AI quests adaptif, AR shadows, guild co-op). (Catatan: Jika belum diupload, tambahkan dari respons Grok.)
- **[Claude](https://raw.githubusercontent.com/aiksatria/sololeveling/main/claude)**: Arsitektur 6-layer granular dengan engine metafisika detail (rumus Bazi/ZWDS/QMDJ), fitur eksklusif seperti Resonance Score, Social Pillar System, Progression Memory, dan Adaptive Difficulty Scaling.

Tim akan blend konsep ini jadi implementasi final. Kontribusi welcome via PR!

## Arsitektur Teknis
- **Frontend**: Kotlin + Jetpack Compose (UI reaktif).
- **Backend**: Pure functions untuk metafisika (BaziCalculator, dll.), Room/SQLite untuk data lokal.
- **Deployment**: Android-only saat ini, potensi cross-platform via KMP.

## Roadmap (Diupdate Februari 2026)
- **MVP (Q1 2026)**: Core stats + daily quests (integrasi Bazi + Qi Men). (Status: Sedang dikerjakan berdasarkan konsep AI.)
- **V1 (Q2 2026)**: Timeline simulator + enemy generator.
- **V2 (Q3 2026)**: AI personalisasi + komunitas features.
- **Beta Testing**: Via Play Store Beta, target 100 user awal.
- **Monetisasi**: Freemium (premium untuk custom themes/shadows).

## Instruksi Kontribusi (Cara Berkontribusi)
Untuk berkontribusi, ikuti langkah-langkah ini secara ketat agar proses review lancar. Kami prioritaskan kontribusi yang menjaga akurasi matematis dan validasi ahli.

1. **Fork Repo**: Klik tombol "Fork" di halaman GitHub repo ini untuk membuat salinan repo di akunmu.
2. **Clone Repo Lokal**: Jalankan `git clone https://github.com/username-mu/sololeveling.git` (ganti dengan URL fork-mu).
3. **Buat Branch Baru**: Selalu buat branch spesifik untuk fitur/bugfix, e.g., `git checkout -b feature/tambah-quest-ai` atau `git checkout -b bugfix/fix-normalisasi-rumus`.
4. **Kerjakan Perubahan**:
   - Pastikan kode Kotlin sesuai standar (gunakan Lint untuk check).
   - Jika tambah rumus matematis, dokumentasikan di komentar kode dan update bagian "Model Matematis" di README jika relevan.
   - Test lokal: Jalankan app di emulator/device, verifikasi output (misal, bandingkan dengan kalkulator manual Bazi).
5. **Commit Changes**: Gunakan pesan commit deskriptif, e.g., `git commit -m 'Tambah fitur AI quest adaptif berdasarkan konsep Grok'`.
6. **Push ke Branch**: `git push origin feature/tambah-quest-ai`.
7. **Buat Pull Request (PR)**:
   - Buka PR ke branch `main` repo asli.
   - Deskripsikan perubahan: Apa yang ditambahkan, mengapa, dan referensi konsep AI mana (jika ada).
   - Sertakan screenshot/test result jika UI/UX berubah.
   - Tag reviewer (misal @aiksatria) jika perlu.
8. **Review dan Merge**: Tim akan review. Jika ada feedback, update branch-mu dan push lagi.

**Aturan Tambahan**:
- **Issue Pertama**: Sebelum kontribusi besar, buka Issue untuk diskusi ide (label: enhancement, bug, dll.).
- **Validasi**: Semua rumus baru harus open-source, verifiable (sertakan sumber/referensi), dan bisa diaudit ahli. Jika metafisika, link ke buku/standar Tiongkok klasik.
- **Code Style**: Ikuti Kotlin conventions (indentasi 4 spasi, no trailing whitespace).
- **Lisensi**: Kontribusi otomatis di bawah MIT – pastikan kode orisinal.
- **Pertanyaan**: Diskusi di Issue atau X (@ismayadewamitra).

## Lisensi
MIT License – bebas pakai/modifikasi, tapi kredit ke repo asli.
