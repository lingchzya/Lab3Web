# Laporan Praktikum 3 - CSS Dasar

**Mata Kuliah:** Pemrograman Web  
**Dosen Pengampu:** Agung Nugroho, M.Kom  
**Universitas:** Universitas Pelita Bangsa  

---

## Langkah-Langkah Praktikum

### 1. Membuat Struktur Dokumen HTML
Membuat file `lab2_css_dasar.html` dengan struktur dasar elemen HTML, header, navigasi, dan konten teks.

![Tampilan HTML Dasar](img/1_html_dasar.png)

### 2. Mendeklarasikan CSS Internal
Menambahkan tag `<style>` pada bagian `<head>` untuk memberikan penataan font pada `body`, border pada `header`, serta warna dan ukuran font pada `h1`.

![Penambahan Internal CSS](img/2_css_internal.png)

### 3. Menambahkan Inline CSS
Menambahkan atribut `style` langsung pada tag `<p>` untuk mengubah warna teks dan perataan paragraf.

![Penambahan Inline CSS](img/3_inline_css.png)

### 4. Membuat CSS Eksternal
Membuat file terpisah `style_eksternal.css` untuk mengatur bagian `<nav>` dan merujuknya menggunakan tag `<link rel="stylesheet">` pada dokumen HTML.

![Tampilan Eksternal CSS](img/4_css_eksternal.png)

### 5. Menambahkan CSS Selector (ID dan Class)
Menerapkan **ID Selector** (`#intro`) untuk styling kotak informasi dan **Class Selector** (`.button`, `.btn-primary`) untuk membuat komponen tombol interaktif.

![Tampilan Akhir Praktikum](img/5_css_selector.png)

---

## Jawaban Pertanyaan dan Tugas

### 1. Eksperimen CSS
Properti dan nilai telah dimodifikasi menggunakan paduan warna latar belakang, tombol interaktif, dan penataan navigasi sesuai instruksi CSS Cheat Sheet.

### 2. Perbedaan `h1 {...}` dan `#intro h1 {...}`
* **`h1 {...}`**: Bersifat global, mengubah tampilan seluruh tag `<h1>` pada dokumen HTML.
* **`#intro h1 {...}`**: Bersifat spesifik, hanya mengubah tag `<h1>` yang berada di dalam elemen yang memiliki `id="intro"`.

### 3. Prioritas Deklarasi CSS (Internal, Eksternal, dan Inline)
Aturan CSS yang diprioritaskan oleh browser adalah **Inline CSS** (atribut `style` di dalam tag HTML).  
*Urutan prioritas dari tertinggi ke terendah:*  
1. Inline CSS  
2. Internal/External CSS (ditentukan oleh urutan kode paling bawah)  
3. Browser Default  

### 4. Prioritas ID Selector vs Class Selector
Browser akan memprioritaskan **ID Selector** karena memiliki bobot spesifisitas (*specificity*) yang lebih tinggi (`0,1,0,0`) dibandingkan Class Selector (`0,0,1,0`).  
*Contoh:* Untuk tag `<p id="paragraf-1" class="text-paragraf">`, gaya yang ditulis pada `#paragraf-1` akan menimpa gaya pada `.text-paragraf`.
