# Dummy Web Prototype Roadmap

## Project Intent

- Bangun dummy web application high-fidelity untuk memvalidasi requirement dan design sebelum development Flutter penuh dimulai.
- Gunakan front-end code dengan data statis realistis agar stakeholder bisa menilai alur dan konten aplikasi secara menyeluruh.【F:JejakAnak - Dummy Prototype Master Plan.md†L5-L22】

## Sukses Ditandai Oleh

- Semua user flow utama dapat dijalankan dari awal hingga akhir oleh tester.
- Tim psikolog, Uwa Farah, dan parent testers merasa pengalaman edukatif dan alur konten sesuai kebutuhan.
- Tim teknis yakin requirement dapat diimplementasikan dalam versi produksi.【F:JejakAnak - Dummy Prototype Master Plan.md†L26-L63】

## Batasan Prototype

- Tidak ada backend, autentikasi, upload foto, atau perhitungan gamifikasi nyata.
- Fokus pada interaksi UI/UX; keamanan dan performa bukan prioritas pada fase ini.【F:JejakAnak - Dummy Prototype Master Plan.md†L64-L71】

## Cakupan Layar

### Must Have (Core Flow)

1. Splash & onboarding carousel.
2. Sign up/login mock.
3. Profil orang tua dan penambahan anak (2 langkah + personalisasi).
4. Home dashboard dengan rekomendasi, jadwal, statistik singkat, dan memori terbaru.
5. Activity library, detail, serta modal penjadwalan.
6. Log activity 3 langkah, timeline anak, dan dashboard insight anak.【F:JejakAnak - Dummy Prototype Master Plan.md†L75-L103】

### Should Have

- Settings & edit profile.
- Jadwal aktivitas (list/calendar).
- Penjelasan rekomendasi, badge showcase, challenge page.
- Play spot detail sederhana dan halaman FAQ.【F:JejakAnak - Dummy Prototype Master Plan.md†L104-L113】

### Nice to Have

- Admin dashboard, pembuatan aktivitas, review queue.
- Activity variations dan recipe exchange untuk konten komunitas.【F:JejakAnak - Dummy Prototype Master Plan.md†L115-L121】

## User Flow Prioritas

1. **First-Time Onboarding** → Splash → Onboarding slides → Sign up → Profil orang tua → Tambah anak → Personalisasi → Home dashboard.
2. **Browse & Schedule Activity** → Home dashboard → Pilih aktivitas rekomendasi → Activity detail → Jadwalkan.
3. **Log Activity & Review Progress** → Home dashboard → Log aktivitas → Isi catatan & 4E feedback → Timeline anak → Dashboard insight.
   Flow ini perlu divisualisasikan dalam prototype agar stakeholder dapat mengevaluasi kelancaran tiap langkah.【F:JejakAnak - Dummy Prototype Master Plan.md†L125-L170】

## Rekomendasi Implementasi

- Gunakan framework komponen web (mis. Next.js/React + Tailwind) dengan routing multipage untuk memudahkan simulasi layar.
- Simpan dummy data (anak, aktivitas, jadwal) sebagai file JSON lokal yang di-load pada saat build.
- Siapkan utilitas untuk toggle state (mis. `useState`/context) yang mensimulasikan login, pemilihan anak, dan status aktivitas tanpa backend.
- Sertakan file konfigurasi data terpisah agar tim konten mudah mengedit placeholder aktivitas.

## Rencana Sprint (3 Minggu)

- **Minggu 1**: Setup project, desain ulang style-guide dasar, implementasi flow onboarding & account setup.
- **Minggu 2**: Bangun dashboard, library aktivitas, dan modal penjadwalan dengan dummy data lengkap.
- **Minggu 3**: Implementasi logging, timeline, insight anak, serta finishing touch (should have + polish). Lakukan sesi validasi & catat feedback.

## Artefak Pendukung

- Pastikan setiap iterasi menghasilkan recording atau catatan feedback dari stakeholder.
- Dokumentasikan perubahan requirement yang muncul selama pengujian prototype untuk dibawa ke fase development berikutnya.
