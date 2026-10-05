# Delta final project - JCBDAAH 006
# Bank marketing campaigns dataset analysis

Proyek ini dibuat untuk menganalisis conversion rate telemarketing yang dilakukan oleh Bank Portugal
periode 2008-2010 pada saat awal krisis global yang hanya mencapai 11,3% tingkat keberhasilannya.
Telemarketing dilakukan oleh Bank untuk menawarkan produk deposito berjangka kepada nasabah.

# Project overview
Pada proyek ini dilakukan metode analisa deskriptif terhadap history/riwayat telemarketing untuk meneliti
pola atau faktor apa yang bisa mempengaruhi keberhasilan nasabah tertarik dengan penawaran deposito berjangka
yang meliputi 3 faktor utama: Demografi nasabah, riwayat telemarketing, dan faktor/kondisi sosial ekonomi

# Dataset
41188 baris dengan 20 kolom

tidak ada data tahun, hanya hari dan bulan

tidak ada unique ID/ primary key

hasil data menjadi sangat tidak seimbang

# Data dictionary
A. Data Nasabah
| Kolom | Tipe Data | Deskripsi |
|---|---|---|
| age | numerik | Umur nasabah dalam tahun |
| job | kategori | Jenis pekerjaan nasabah: admin, blue-collar, entrepreneur, management, retired, student, technician, housemaid, services, unemployed, self-employed dan unknown |
| marital | kategori | Status pernikahan nasabah: married, single, divorced, atau unknown |
| education | kategori | Tingkat pendidikan nasabah, antara lain basic.4y, basic.6y, basic.9y, high.school, professional.course, university.degree, illiterate, atau unknown |
| default | kategori | Status apakah nasabah memiliki status kredit macet <br><br> yes = ya, kredit macet <br> no = tidak ada kredit macet/lancar <br> unknown = tidak tahu |
| housing | kategori | Status kepemilikan kredit rumah atau KPR <br><br> yes = punya KPR <br>no = tidak punya KPR <br> unknown = tidak tahu |
| loan | kategori | Status kepemilikan pinjaman pribadi <br><br> yes = punya pinjaman <br> no = tidak ada pinjaman <br> unknown = tidak tahu |
---
B. Informasi/riwayat kontak terakhir pada masa kampanye berjalan
| Kolom | Tipe Data | Deskripsi |
|---|---|---|
| contact | kategori | Saluran komunikasi yang digunakan untuk menghubungi nasabah: cellular atau telephone |
| month | kategori | Bulan ketika panggilan terakhir dilakukan, hanya 10 bulan dalam setahun, tidak ada januari dan februari
| day_of_week | kategori | Hari (5 hari kerja) ketika panggilan terakhir dilakukan: mon, tue, wed, thu, atau fri |
| duration | numerik | Durasi panggilan terakhir dalam satuan detik |
| campaign | numerik | Jumlah panggilan yang dilakukan pada masa kampanye ini, termasuk kontak terakhir |
---
C. Informasi/riwayat kontak terkait dengan masa kampanye sebelumnya
| Kolom | Tipe Data | Deskripsi |
|---|---|---|
| pdays | numerik | Jumlah hari sejak nasabah terakhir kali dihubungi pada kampanye sebelumnya; nilai 999 berarti nasabah belum pernah dihubungi sebelumnya |
| previous | numerik | Jumlah panggilan yang dilakukan kepada nasabah sebelum kampanye berjalan |
| poutcome | kategori | Hasil kampanye pemasaran sebelumnya <br><br>success = berhasil<br>failure = gagal<br>nonexistent = tidak diketahui |
---
D. Kondisi sosial dan ekonomi (kondisi makro ekonomi) saat dihubungi
| Kolom | Tipe Data | Deskripsi |
|---|---|---|
| emp.var.rate | numerik | Employment variation rate, yaitu indikator perubahan tingkat ketenagakerjaan per kuartal |
| cons.price.idx | numerik |Consumer price index atau indeks harga konsumen bulanan |
| cons.conf.idx | numerik | Consumer confidence index atau indeks kepercayaan konsumen bulanan |
| euribor3m | numerik | Suku bunga Euribor tenor 3 bulan yang dicatat secara harian |
| nr.employed | numerik | Jumlah tenaga kerja sebagai indikator ekonomi kuartalan |
---
E. Hasil akhir
| Kolom | Tipe Data | Deskripsi |
|---|---|---|
| y | Tipe Data | Target apakah nasabah akhirnya membuka term deposit: yes atau no |

# Hasil temuan
Setelah diberi fitur tahun, data terlihat secara kronolgis dari 2008-2010. Maka akan terlihat di awal 2008, Bank melakukan marketing secara masif menyebabkan conversion rate menjadi rendah. Pada pertengahan 2008 hingga awal 2009 terlihat Bank mulai melakukan perubahan sehingga mulai memperlihatkan conversion rate yang meningkat, hingga akhir 2010 terlihat Bank secara konsisten memperlihatkan conversion rate mencapai 60%.

Analisa dilakukan untuk mengidentifikasi faktor-faktor yang mempengaruhi keberhasilan atau peningkatan conversion rate

# Cara Menjalankan project
1. download repository
2. download file dataset di: https://www.kaggle.com/datasets/volodymyrgavrysh/bank-marketing-campaigns-dataset
3. Buka file notebook yang di-download dari repository
4. Jalankan semua cell dari awal sampai akhir



# source: https://www.kaggle.com/datasets/volodymyrgavrysh/bank-marketing-campaigns-dataset

