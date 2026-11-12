# CODING AGENT RULES

Proyek ini akan dipakai untuk WordPress Elementor HTML Element dan Site Custom CSS. Oleh karena itu, proyek ini WAJIB mengikuti konfigurasi ini:

- Setiap page adalah HTML.
- Setiap HTML page punya JavaScript-nya sendiri dan WAJIB INTERNAL JAVASCRIPT.
- Untuk desain WAJIB pakai CSS EXTERNAL, TIDAK BOLEH CSS INTERNAL dan INLINE.
- Saat membuat Header (Nav) dan Footer, WAJIB DIBUAT HTML TERPISAH. Jangan satukan dengan HTML PAGE.
- Custom Font wajib dari Google Font.
- Mengikuti Aturan Detail di bawah ini.
- Setiap gambar wajib bisa diklik dan memunculkan popup overview di tab yang sama; tidak perlu pindah tab.
- Navbar wajib rounded dengan latar belakang blur transparan.

## Aturan Penulisan Konten

- Jangan pernah mengubah copywriting yang diberikan user.
- Jangan menambahkan atau mengurangi apa pun dari copywriting yang diberikan user.
- Copywriting harus 100% sama karena sudah disesuaikan untuk SEO.

## Aturan Projek

- Pastikan struktur proyek rapi dan tempatkan aset sesuai fungsinya.
- Semua page HTML dan CSS ada di root; jangan masukkan ke dalam subfolder.

## Aturan HTML

- Setiap page = 1 full HTML standalone.
- Wajib mengikuti best practice Semantic HTML agar SEO bagus.
- Wajib mengisi semua ALT IMAGE dengan isi yang sesuai konteksnya.
- Tidak boleh mengimpor Custom Font di HTML karena Custom Font wajib di CSS.
- Tiap link internal untuk pindah antar-page wajib menggunakan `/<slug-page>`, mengikuti prinsip href WordPress Elementor Page. Slug harus sesuai dengan nama page `.html` yang dibuat.
- Untuk external link tidak ada aturan khusus, kecuali harus open in blank page.
- Header dan Footer dipisah dengan membuat `header.html` dan `footer.html`.

## Aturan CSS

- CSS masuk ke Global CSS Elementor yang berlaku sitewide.
- CSS hanya ada satu dan dipakai untuk semua page, termasuk Header dan Footer.
- Ikuti best practice CSS dengan mendefinisikan nilai yang berulang di `:root { --<property-css> }`.
- Custom Font wajib diimpor dari CSS menggunakan CSS `@import` dari Google Fonts.
- Terapkan breakpoint responsive dengan pendekatan mobile-first.

## Aturan JS

- Semua tag script JS harus inline di dalam tag `<body>` HTML.
- Terapkan Internal JS.
- Tidak ada file `.js` terpisah.
- Dilarang menaruh script di dalam `<head>`.

## Aturan Accessibility dan Performa

- Semua `<img>` wajib memiliki atribut `alt` dengan isi yang sesuai konteks.
- Gunakan `loading="lazy"` untuk semua gambar kecuali gambar LCP (hero above the fold).
- Semua `<img>` wajib memiliki atribut `width` dan `height` untuk mencegah layout shift (CLS).
- Gunakan `rel="preload"` untuk aset kritis.

## List Link/Informasi External

Link yang akan dipakai dan saya masukkan di copywriting wajib digunakan. Kalau link kosong berarti memang tidak ada. Kalau ada isinya, pastikan dipakai.

## FOOTER

- Ikon media sosial wajib menggunakan SVG. Link media sosial akan saya berikan di copywriting.
