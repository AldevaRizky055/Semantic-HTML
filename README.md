Menggunakan CSS (Cascading Style Sheets) dalam sebuah halaman HTML membawa perbedaan yang signifikan pada penampilan dan tata letak halaman dibandingkan dengan hanya menggunakan HTML tanpa CSS. Berikut ini adalah penjelasan lengkap perbedaan antara menggunakan CSS dan tidak menggunakan CSS dari program di atas.

### 1. **Tampilan Visual**
- **Tanpa CSS**: 
  - Halaman HTML tanpa CSS akan menampilkan elemen-elemen secara sederhana dan default. Semua elemen HTML akan terlihat dalam tata letak linier dari atas ke bawah, tanpa ada penyesuaian warna, ukuran, atau posisi.
  - Header, navigasi, konten, dan footer akan tampil dalam urutan blok satu di bawah yang lain dengan tampilan standar hitam-putih.
- **Dengan CSS**: 
  - Elemen-elemen halaman dapat diatur sedemikian rupa dengan berbagai atribut visual, seperti warna latar belakang, margin, padding, tata letak grid, dan lain-lain.
  - Dalam contoh Anda, penggunaan CSS memberikan warna latar yang berbeda pada setiap elemen (`header`, `nav`, `section`, `footer`), menambahkan padding untuk jarak antar elemen, dan membuat tata letak grid yang memposisikan `nav` di sebelah kiri dan `section` di tengah.

### 2. **Tata Letak Halaman**
- **Tanpa CSS**: 
  - Semua elemen HTML ditampilkan secara vertikal dalam satu kolom. Tidak ada pengaturan posisi elemen yang fleksibel, sehingga halaman cenderung terlihat monoton dan tidak menarik.
- **Dengan CSS**: 
  - CSS memungkinkan penggunaan **grid layout** yang dapat mengatur elemen-elemen secara responsif dan lebih terstruktur. Dalam contoh Anda, CSS membuat elemen-elemen memiliki area grid yang berbeda:
    ```css
    body {
        display: grid;
        grid-template-areas:
            "header header header"
            "nav section section"
            "footer footer footer";
        grid-template-rows: 80px 1fr 50px;
        grid-template-columns: 20% 1fr 18%;
    }
    ```
    Ini membuat `header` berada di bagian atas, `nav` di sebelah kiri, `section` di tengah, dan `footer` di bagian bawah, memberikan struktur halaman yang lebih profesional.

### 3. **Warna dan Gaya Visual**
- **Tanpa CSS**: 
  - Warna elemen dan teks akan ditampilkan sesuai dengan pengaturan default browser, yaitu teks hitam dengan latar belakang putih atau abu-abu.
- **Dengan CSS**: 
  - Elemen-elemen dapat diubah warnanya sesuai kebutuhan. Contohnya, `header` dan `footer` diberi warna abu-abu gelap, `nav` diberi warna abu-abu muda, dan `section` memiliki warna abu-abu netral.
    ```css
    header {
        background: #707070;
    }
    nav {
        background: #C9BFBF;
    }
    section {
        background: #ABABAB;
    }
    footer {
        background: #707070;
    }
    ```

### 4. **Ukuran dan Spasi Antar Elemen**
- **Tanpa CSS**:
  - Elemen-elemen akan ditampilkan dengan margin dan padding default yang seringkali tidak memadai untuk tampilan estetis.
- **Dengan CSS**:
  - Anda dapat menambahkan margin, padding, dan spasi antar elemen untuk memberikan kesan ruang yang lebih lega dan rapi. Contoh:
    ```css
    header, nav, section, footer {
        padding: 5px;
    }
    ```

### 5. **Responsivitas**
- **Tanpa CSS**:
  - Elemen-elemen tidak akan secara otomatis menyesuaikan diri dengan ukuran layar perangkat. Halaman akan terlihat sama pada layar kecil maupun besar, tanpa adaptasi.
- **Dengan CSS**:
  - CSS dapat digunakan untuk membuat tata letak yang responsif, yang berarti halaman akan menyesuaikan diri sesuai ukuran layar perangkat. Misalnya, penggunaan **grid layout** seperti pada contoh Anda membantu halaman untuk menampilkan elemen-elemen dengan proporsi yang lebih seimbang di berbagai ukuran layar.

### **Kesimpulan**
CSS sangat penting dalam membuat halaman web yang menarik, terstruktur, dan user-friendly. Tanpa CSS, halaman web cenderung terlihat polos, tidak terstruktur, dan kurang menarik secara visual. Dengan CSS, halaman web dapat diubah menjadi sesuatu yang lebih interaktif dan modern, dengan tata letak, warna, dan elemen visual yang sesuai dengan kebutuhan pengguna.