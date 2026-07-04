# Superstore-Sales-Analysis
📊 Superstore Sales Analysis Dashboard
https://public.tableau.com/views/SuperstoreDataAnalystProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

📖 Tentang Proyek Ini

Proyek ini adalah analisis data penjualan dari sebuah toko ritel besar (Superstore) untuk memahami performa bisnis dan memberikan rekomendasi strategis. Tujuannya adalah mengubah data mentah menjadi wawasan yang dapat ditindaklanjuti terkait penjualan, keuntungan, dan perilaku pelanggan .

🗂️ Dataset: Menggunakan dataset publik Sample - Superstore yang berisi data penjualan dari tahun 2014–2017 di berbagai wilayah AS. Dataset ini mencakup informasi tentang pesanan, pelanggan, produk, dan metrik keuangan .
🔍 Insight & Temuan Utama

📊 1. Performa Penjualan per Kategori & Sub-Kategori

Pertanyaan: Kategori apa yang paling laris dan paling untung?

Kategori Total Penjualan (Rp) Total Profit (Rp) Profit Margin
Teknologi $872,745 $95,862 11.0%
Perlengkapan Kantor $798,889 $87,415 10.9%
Furniture $660,381 -$47,455 -7.2%

🔎 Insight:

· Teknologi adalah kategori dengan penjualan tertinggi ($872,745)** dan profit tertinggi **($95,862).
· Furniture menjadi perhatian utama karena merugi ($47,455) meskipun penjualannya cukup tinggi. Ini mengindikasikan adanya masalah pada harga pokok penjualan atau strategi diskon yang tidak tepat .
· Sub-Kategori Terlaris:
  · Phones ($330,007) dan **Chairs** ($328,430) mendominasi penjualan.
  · Tables menjadi sub-kategori dengan profit negatif terbesar (-$17,725).

---

🗺️ 2. Distribusi Penjualan & Profit per Wilayah

Pertanyaan: Region mana yang performa terbaik/terburuk?

Region Total Penjualan Total Profit Kontribusi
West $742,919 $17,469 31.9%
East $695,776 $7,695 29.9%
Central $501,239 $7,395 21.5%
South $391,722 $2,263 16.8%

🔎 Insight:

· Wilayah West memimpin penjualan dan profit, terutama didorong oleh California yang menyumbang $471,811 atau 63.5% dari total penjualan West .
· Wilayah South memiliki performa terendah (hanya 16.8% kontribusi) dengan profit paling tipis ($2,263). Ini menjadi peluang ekspansi terbesar .
· Top 5 Negara Bagian:
  1. California ($471,811)
  2. New York ($308,738)
  3. Texas ($169,889)
  4. Washington ($147,425)
  5. Pennsylvania ($123,930)

---

📈 3. Tren Penjualan Bulanan & Musiman

Pertanyaan: Bulan apa puncak penjualan? Apakah ada pola musiman?

🔎 Insight:

· Puncak Penjualan:
  · November ($197,931) dan **Desember** ($186,703) menjadi bulan tertinggi, didorong oleh musim liburan dan belanja akhir tahun.
  · Lonjakan signifikan terjadi di September dan November, kemungkinan terkait dengan back-to-school dan Black Friday .
· Penurunan: Penjualan terendah terjadi pada Januari ($73,935) setelah lonjakan liburan.
· Pertumbuhan Tahunan: Penjualan meningkat 47.45% dari 2014 ($484,247) ke 2017 ($713,990).

---

🎯 4. Segmentasi Pelanggan

Pertanyaan: Segmen pelanggan mana paling menguntungkan?

Segment Total Sales Total Profit 
Consumer $1,161,401 $31,343
Corporate $706,146 $35,233
Home Office $429,653 $16,953

🔎 Insight:

· Consumer adalah segmen dengan penjualan tertinggi ($1.16 juta), namun **Corporate** memiliki profit lebih tinggi ($35,233) dengan volume lebih rendah. Ini menunjukkan pelanggan Corporate lebih efisien dan bernilai .
🛠️ Tools & Teknologi

· Data Preparation & Cleaning: Excel (Power Query) 
· Analisis & Dashboard: Excel (Pivot Table, Pivot Chart, Slicer) / Tableau (visualisasi interaktif, peta geografis) 
· Hosting: GitHub (repository ini)


📋 Langkah-Langkah Pengerjaan

Proyek ini dikerjakan melalui 4[Sample - Superstore.csv](https://github.com/user-attachments/files/29661008/Sample.-.Superstore.csv)
[Project Data Analyst Superstore.xlsx](https://github.com/user-attachments/files/29661004/Project.Data.Analyst.Superstore.xlsx)
 tahap utama, dari persiapan data hingga dashboard interaktif.

---

🔧 TAHAP 1: EKSPLORASI & PEMBERSIHAN DATA (Excel)

Tujuan: Memastikan data siap analisis, tidak ada error atau nilai kosong.

Langkah Tugas Output
1 Buka file Sample - Superstore.csv di Excel Data terbuka (9.994 baris x 21 kolom)
2 Cek struktur dan arti tiap kolom Pahami variabel yang tersedia
3 Cek Missing Values: Gunakan CTRL + Shift + ↓ lalu CTRL + F cari nilai kosong Tidak ada missing di kolom kunci (Order ID, Sales, Profit)
4 Cek Duplikat: Pilih kolom Order ID → Conditional Formatting → Highlight Duplicate Values Tidak ada duplikat transaksi
5 Format Data: Pastikan Order Date & Ship Date berformat Date, Sales & Profit berformat Number dengan 2 desimal Data siap diolah
6 Tambahkan Kolom Baru:  - Year = =YEAR([Order Date])  - Month = =MONTH([Order Date])  - Profit Margin = Profit / Sales  - Day Name = =TEXT([Order Date],"dddd") Kolom tambahan untuk analisis lebih dalam

---

📊 TAHAP 2: ANALISIS EKSPLORATORI (Excel Pivot Table)

Tujuan: Dapatkan insight awal dengan Pivot Table untuk menjawab pertanyaan bisnis.

Pivot Table Rows Values Pertanyaan yang Dijawab
1 Category Sales (SUM), Profit (SUM) Kategori apa paling laris dan paling untung?
2 Region Sales (SUM), Profit (SUM) Region mana performa terbaik/terburuk?
3 Order Date (group by Month) Sales (SUM) Bulan apa puncak penjualan?
4 Segment Sales (SUM), Profit (SUM) Segmen pelanggan mana paling menguntungkan?
5 State Sales (SUM) Negara bagian mana kontribusi terbesar?

Hasil: Insight awal yang menjadi dasar untuk visualisasi dan rekomendasi.



---

🎨 TAHAP 3: DASHBOARD INTERAKTIF (Excel)


🚀 TAHAP 4: VISUALISASI LANJUTAN (Tableau)
https://public.tableau.com/views/SuperstoreDataAnalystProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
s:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Su&#47;SuperstoreDataAnalystProject&#47;Dashboard1&#47;1.p

<img width="480" height="305" alt="image" src="https://github.com/user-attachments/assets/95a3fdfd-6459-4ea9-afad-f569e2bb9b78" />



Terimakasih
