# Panduan Penggunaan File HTML & CSS di WordPress Elementor

Folder `elementor/` ini berisi template HTML dan CSS siap pakai yang dirancang khusus untuk widget **HTML Code Elementor** dan **Site Custom CSS Elementor**.

Semua file telah dioptimalkan agar:
- Tidak ada duplikasi tag `<!DOCTYPE>`, `<html>`, atau `<head>` saat ditempel ke dalam WordPress.
- Internal JavaScript sudah otomatis terpasang di masing-masing file (FAQ accordion, mobile menu toggle, lightbox popup overview).
- Desain 100% responsif di desktop, tablet, dan mobile.
- Copywriting dan link sesuai SEO 100% tanpa perubahan.

---

## 📁 Daftar File di Dalam Folder `elementor/`

| Nama File | Fungsi | Lokasi Pemasangan di WordPress |
| :--- | :--- | :--- |
| **`style-sitewide-elementor.css`** | Global CSS Sitewide (Desain, font, gradien, glassmorphism) | **Elementor > Site Settings > Custom CSS** atau **Appearance > Customize > Additional CSS** |
| **`header-elementor.html`** | Header navigasi rounded transparan + mobile drawer | **Templates > Theme Builder > Header** (Widget HTML) |
| **`footer-elementor.html`** | Footer 3-kolom responsif + ikon SVG Meta Threads + Back to Top | **Templates > Theme Builder > Footer** (Widget HTML) |
| **`home-elementor.html`** | Halaman utama Kaya Chat | **Pages > Home** (Widget HTML) |
| **`host-elementor.html`** | Halaman pendaftaran & panduan Host | **Pages > Host** (Widget HTML) |
| **`agent-elementor.html`** | Halaman pendaftaran & panduan Agency | **Pages > Agent** (Widget HTML) |
| **`contact-elementor.html`** | Halaman kontak & channel resmi support | **Pages > Contact** (Widget HTML) |

---

## 🚀 Langkah-langkah Pemasangan di WordPress Elementor

### Langkah 1: Pasang Global CSS (Hanya Perlu 1 Kali)
1. Buka dashboard WordPress Anda.
2. Buka salah satu halaman dengan Elementor (atau buka **Elementor > Site Settings** dari hamburger menu kiri atas editor Elementor).
3. Masuk ke menu **Custom CSS**.
   *(Atau dari Dashboard WP: **Appearance (Tampilan) > Customize (Sesuaikan) > Additional CSS**)*.
4. Buka file **`style-sitewide-elementor.css`**, copy seluruh isinya, lalu paste ke kotak CSS tersebut.
5. Klik **Update / Publish**.

---

### Langkah 2: Buat Header di Elementor Theme Builder
1. Di Dashboard WP, masuk ke **Templates > Theme Builder > Header > Add New**.
2. Masukkan section 1 kolom **Full Width** (*Content Width: Full Width, Column Gap: No Gap*).
3. Tarik widget **HTML** Elementor ke dalam section tersebut.
4. Buka file **`header-elementor.html`**, copy seluruh isinya, dan paste ke dalam widget HTML.
5. Klik **Publish**, lalu atur kondisi tampilan (*Display Conditions*) ke: **Entire Site**.

---

### Langkah 3: Buat Footer di Elementor Theme Builder
1. Di Dashboard WP, masuk ke **Templates > Theme Builder > Footer > Add New**.
2. Masukkan section 1 kolom **Full Width** (*Content Width: Full Width, Column Gap: No Gap*).
3. Tarik widget **HTML** Elementor ke dalam section tersebut.
4. Buka file **`footer-elementor.html`**, copy seluruh isinya, dan paste ke dalam widget HTML.
5. Klik **Publish**, lalu atur kondisi tampilan (*Display Conditions*) ke: **Entire Site**.

---

### Langkah 4: Buat Halaman (Home, Host, Agent, Contact)

Pastikan Permalink WordPress Anda sudah diset ke **Post name** di **Settings > Permalinks** agar slug link internal (`/host`, `/agent`, `/contact`) berjalan mulus.

#### 1. Halaman Home (`/`)
- Buat halaman baru di **Pages > Add New**, beri judul **Home**.
- Di pengaturan halaman Elementor (ikon gerigi kiri bawah), pilih **Page Layout: Elementor Full Width**.
- Tarik widget **HTML** Elementor ke section full width.
- Copy seluruh isi file **`home-elementor.html`** dan paste ke widget HTML.
- Klik **Publish**.
- Di **Settings > Reading**, setel *"Your homepage displays"* ke *A static page* &rarr; pilih halaman Home yang baru dibuat.

#### 2. Halaman Host (`/host`)
- Buat halaman baru dengan slug permalink: **`host`**.
- Buka dengan Elementor, setel **Page Layout: Elementor Full Width**.
- Tarik widget **HTML** Elementor.
- Copy seluruh isi file **`host-elementor.html`** dan paste ke widget HTML.
- Klik **Publish**.

#### 3. Halaman Agent (`/agent`)
- Buat halaman baru dengan slug permalink: **`agent`**.
- Buka dengan Elementor, setel **Page Layout: Elementor Full Width**.
- Tarik widget **HTML** Elementor.
- Copy seluruh isi file **`agent-elementor.html`** dan paste ke widget HTML.
- Klik **Publish**.

#### 4. Halaman Contact (`/contact`)
- Buat halaman baru dengan slug permalink: **`contact`**.
- Buka dengan Elementor, setel **Page Layout: Elementor Full Width**.
- Tarik widget **HTML** Elementor.
- Copy seluruh isi file **`contact-elementor.html`** dan paste ke widget HTML.
- Klik **Publish**.

---

## ✨ Fitur & Aturan yang Sudah Tertanam Otomatis
- **Lightbox Image Overview**: Setiap gambar dapat diklik dan langsung memunculkan modal popup preview berlatar gelap transparan di tab yang sama tanpa membuka tab baru.
- **Accordion FAQ Interaktif**: Pertanyaan FAQ dapat diklik untuk membuka/menutup jawaban dengan animasi halus.
- **Mobile Menu Drawer**: Menu mobile adaptif dengan tombol hamburger, efek glassmorphism, dan penutup otomatis jika pengguna mengklik di luar menu atau menekan tombol `Esc`.
- **Back to Top Smooth Scroll**: Tombol kembali ke atas di footer menggulir layar secara mulus.
- **SEO & Performa**: Semua `<img>` dilengkapi tag alt kontekstual, dimensi `width` dan `height` untuk mencegah CLS, serta `loading="lazy"` pada gambar di bawah hero.

