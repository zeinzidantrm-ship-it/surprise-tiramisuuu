# A Little Surprise 💌

Website kejutan personal untuk Tiramisuuu — dibuat dengan HTML, CSS, dan JS murni (tanpa framework/build tool), jadi tinggal buka `index.html` dan langsung jalan.

## Struktur folder

```
surprise-tiramisuuu/
├── index.html          # semua halaman (landing, menu, journey, moments) ada di sini
├── assets/
│   ├── img/             # foto-foto untuk galeri di halaman Moments
│   │   ├── moment-1.jpg
│   │   ├── moment-2.jpg
│   │   ├── moment-3.jpg
│   │   ├── moment-4.jpg
│   │   └── moment-5.jpg
│   └── video/
│       └── moments.mp4  # video montage di halaman Moments
└── README.md
```

## Cara buka di lokal

Tinggal double-click `index.html`, atau kalau mau lewat local server (disarankan supaya video/gambar pasti kebaca):

```bash
# dari dalam folder surprise-tiramisuuu/
python3 -m http.server 8000
# lalu buka http://localhost:8000 di browser
```

Atau pakai extension **Live Server** di VS Code (klik kanan `index.html` → "Open with Live Server").

## Cara edit

- **Teks timeline "Journey"** — buka `index.html`, cari komentar `EDIT YOUR TIMELINE HERE` di bagian `<script>` paling bawah. Tinggal ganti `date` dan `text` di array `timelineData`, boleh tambah/kurangi item.
- **Foto di halaman Moments** — ganti file di `assets/img/` (pertahankan nama file yang sama, atau update path `src` di HTML kalau nama filenya beda).
- **Video di halaman Moments** — ganti file `assets/video/moments.mp4` dengan video lain (nama file harus sama, atau update path `src`-nya).
- **Lagu latar** — cari `YT_ID` di bagian `<script>`, ganti dengan video ID YouTube lain kalau mau ganti lagu.

## Deploy gratis ke GitHub Pages

1. Push folder ini ke repository GitHub kamu.
2. Buka repo → **Settings** → **Pages**.
3. Di **Source**, pilih branch `main` dan folder `/ (root)`.
4. Save — link live-nya akan muncul di halaman yang sama setelah beberapa menit (format: `https://<username>.github.io/<nama-repo>/`).

## Catatan

Video dan foto di `assets/` adalah file pribadi — pastikan repo-nya **private** di GitHub kalau kontennya nggak untuk konsumsi publik.
