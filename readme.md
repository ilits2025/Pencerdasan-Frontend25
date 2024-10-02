# Pencerdasan Frontend ILITS 2025

## Tech Stack

- Typescript
- Next.js v14
- TailwindCSS
- React Query (Query Management)
- React Hook Forms (Form Management)
- zod (Schema Validation)

## Penjelasan

### Typescript

TypeScript adalah bahasa pemrograman open-source yang dikembangkan oleh Microsoft. TypeScript adalah `superset` dari JavaScript, yang berarti semua sintaksis dan fitur JavaScript juga tersedia di TypeScript, tetapi dengan penambahan kemampuan `tipe` (type) yang lebih kuat.

Kelebihan TypeScript antara lain:

1. Kemampuan tipe yang lebih kuat, sehingga kode menjadi lebih terstruktur dan mudah dipahami, serta memungkinkan untuk mendeteksi kesalahan pada saat kompilasi.
2. Meningkatkan produktivitas pengembang dengan memungkinkan otomatisasi refaktorisasi kode, dukungan untuk refactor yang lebih aman, dan fitur editor IntelliSense yang canggih.
3. TypeScript menawarkan fitur-fitur modern seperti async/await, dekorator, dan banyak lagi.
4. Lebih mudah untuk melakukan debugging kode TypeScript.

### Next.js v14

Next.js adalah kerangka kerja JavaScript sumber terbuka (open source) yang digunakan untuk membuat aplikasi web dengan cepat dan mudah menggunakan React. Next.js dirancang untuk mempercepat proses pengembangan aplikasi web dengan menyediakan fitur-fitur seperti server-side rendering (SSR), pre-rendering, dan optimasi performa.

### TailwindCSS

TailwindCSS adalah framework untuk CSS yang mempermudah dalam melakukan styling CSS dengan lebih cepat dan efisien. Selain itu, TailwindCSS juga bisa membuat custom class untuk setiap component, Tailwind menyediakan kelas utility yang dapat langsung digunakan di HTML. Kelas-kelas ini mencakup margin, padding, ukuran, warna, hingga tata letak responsif, sehingga memudahkan styling tanpa harus membuat stylesheet terpisah.

Kelebihan dari TailwindCSS:

1. **Kecepatan dan Efisiensi**: sehingga mempercepat pengembangan karena tidak perlu beralih ke file CSS.
2. **Konsistensi Desain**: Utility classes memastikan tampilan yang konsisten di seluruh halaman, mengurangi risiko inkonsistensi antar komponen.
3. **Customizable**: Tailwind bisa dikustomisasi melalui konfigurasi, sehingga sesuai dengan kebutuhan desain spesifik proyek tanpa harus menulis ulang banyak kode.
4. **Responsive Design**: Tailwind menyediakan kelas bawaan untuk desain responsif, sehingga memudahkan penyesuaian tampilan di berbagai ukuran layar.

### React Query

Library yang mempermudah pengelolaan data asinkron dalam aplikasi React, terutama saat berurusan dengan API seperti mengatur state, loading, error, dan caching secara manual, React Query menangani semua itu secara otomatis dan menjadi lebih efisien.

Kelebihan:

1. React Query secara otomatis mengurus data fetching, error handling, dan state loading, sehingga kode jadi lebih bersih dan lebih sedikit boilerplate dibanding pengelolaan manual.
2. React Query bisa otomatis me-refresh data ketika dianggap usang atau ada perubahan, memastikan aplikasi selalu menampilkan data terbaru.
3. React Query juga mendukung mutations, yang memudahkan pengiriman data ke server (seperti menambah, mengubah, atau menghapus data). Setelah mutation berhasil, cache otomatis diperbarui, jadi UI selalu sinkron dengan data terbaru.

### React Hook Forms

React Hook Form adalah library untuk menangani form dalam aplikasi React. Library ini memanfaatkan fitur React Hooks sehingga memungkinkan pengelolaan form state, validasi, dan pengiriman data dengan lebih efisien. React Hook Form fokus pada kinerja, sehingga cocok digunakan dalam form yang kompleks dan dengan banyak input.

Kelebihan:

1. React Hook Form bekerja tanpa perlu re-render berlebihan setiap kali ada perubahan input. Ini menjaga performa aplikasi tetap cepat, terutama untuk form yang besar atau kompleks.
2. React Hook Form mendukung integrasi validasi yang mudah, baik menggunakan fitur built-in atau melalui library validasi seperti **Zod**.
3. React Hook Form mendukung penggunaan **controlled** components di form, memberikan fleksibilitas untuk berbagai kebutuhan.
4. Dengan React Hook Form, proses pengiriman data (submit) lebih sederhana, karena semuanya dikelola melalui satu fungsi handleSubmit yang menangani validasi dan pengiriman data secara otomatis.

### Zod

Zod adalah library untuk validasi skema di JavaScript dan TypeScript. Zod dirancang untuk menjadi sederhana, fleksibel, dan mudah digunakan, memungkinkan pengembang untuk mendefinisikan skema data dan melakukan validasi dengan cara yang intuitif. Dengan Zod, kamu dapat memastikan bahwa data yang diterima oleh aplikasi sesuai dengan format yang diharapkan sebelum diproses lebih lanjut.

Kelebihan:

1. Zod menggunakan API yang jelas dan deklaratif, sehingga mudah dipahami. Pengembang dapat mendefinisikan skema validasi dengan cara yang sangat mirip dengan mendeklarasikan tipe data
2. Zod sepenuhnya mendukung TypeScript, memberikan inferensi tipe yang kuat. Hal ini memungkinkan untuk mendapatkan keuntungan dari tiping yang kuat di seluruh aplikasi, mengurangi kemungkinan bug yang disebabkan oleh tipe data yang tidak sesuai.
3. Zod memberikan pesan error yang jelas dan terperinci ketika validasi gagal, sehingga memudahkan dalam memahami dan menangani kesalahan.
4. Zod mudah diintegrasikan dengan framework lain seperti React, membuatnya sangat cocok untuk validasi form. Dengan menggunakan Zod dalam kombinasi dengan library seperti React Hook Form

## Task Frontend

- Merancang dan mengembangkan antarmuka pengguna (UI) yang responsif di berbagai perangkat
- Bekerjasama dengan pihak UI/UX dalam melakukan slicing hasil desain UI
- Bekerjasama dengan pihak Backend dalam melakukan integrasi API
- Menerapkan clean code and best practice dalam proses development
- Memastikan performa website tetap stabil

## Workflow Kerja

1. Convert ticket menjadi issues
2. Create branch dari issues
3. Ikutin langkah yang diberikan
4. Lakukan pull ke branch **main** sebelum push ke branch ticket
5. Push ke branch ticket
6. Create pull request
7. Buat deskripsi dan screenshoot hasil kerja yang dibuat untuk pesan pada pull request

## Pencerdasan Git

- Untuk melakukan

```
git add .
```

- Git Conventional Message

`<type>(optional scope): <description> `

```
git commit -M "feat: add table on landing page"
```

- Pull ke **main** branch untuk menyesuaikan branch local dengan branch dev (menghindari conflict)

```
git pull origin main
```

- Push ke branch sesuai dengan ticket

```
git push -u origin <branch_name>
```

- Menyelesaikan Merge

```
git add .
git merge --continue
```

- Mengatasi proses rebase

```
git add .
git rebase --continue
```

\*lakukan langkah tersebut hingga proses rebase selesai

--
more tips: https://ohshitgit.com/

## Note

- Jangan lupa pull ke branch **main** sebelum push
- JANGAN LANGSUNG PUSH KE BRANCH **prod** & **main**
- Semisal mau ngubah component, **PLISS LIHAT2 LAGI APA COMPONENT YANG DIUBAH MALAH NGEFFECT KE HALAMAN LAIN YANG MENGGUNAKAN COMPONENT TERSEBUT**
