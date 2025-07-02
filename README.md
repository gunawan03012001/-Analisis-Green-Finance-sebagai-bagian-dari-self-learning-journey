# -Analisis-Green-Finance-sebagai-bagian-dari-self-learning-journey
🌱 Analisis Green Finance | Self-Learning Project
Hai, Sobat ETL! 👋

Apa kabar hari ini? Semoga tetap semangat dan sehat selalu yaa 💪

Selamat datang di repository ini — repositori ini dibuat sebagai bagian dari self-learning journey untuk memahami dan menganalisis green finance, atau gampangnya: menganalisis cara keuangan yang digunakan untuk project peduli sama lingkungan 🌍💸

🎯 Tujuan Proyek
Tujuan utama dari proyek ini adalah:

 - Memahami konsep green finance dari sisi data termasuk bagaimana data digunakan untuk mengukur dampak dan risiko proyek berkelanjutan.
 - Melihat analisis green finance berdampak terhadap lingkungan dan sosial yang terukur, dengan fokus pada metrik kunci seperti pengurangan emisi CO2, penciptaan lapangan kerja, dan peningkatan akses energi bersih.
 - Mengeksplorasi bagaimana kita dapat menggunakan data historis untuk memprediksi keberhasilan dan risiko proyek hijau, termasuk penerapan teknik Machine Learning sederhana.
 - Membedah berbagai variabel dalam dataset yang relevan, mulai dari data finansial, lingkungan, hingga sosial-ekonomi, dan memahami interkoneksinya dalam konteks keberlanjutan.

# 1. Deskripsi Green Finance

**Green Finance** adalah pendekatan keuangan yang inovatif yang mengarahkan investasi dan pembiayaan ke proyek-proyek yang memiliki dampak positif dan terukur terhadap lingkungan. Fokus utamanya adalah mendukung transisi global menuju ekonomi rendah karbon dan berkelanjutan. Ini mencakup pembiayaan untuk berbagai inisiatif, antara lain:

- Energi Terbarukan: Investasi pada pembangkit listrik tenaga surya (PLTS), pembangkit listrik tenaga mikrohidro (PLTM), angin, panas bumi, dan biomassa.

- Pengelolaan Limbah Berkelanjutan: Proyek-proyek yang berfokus pada daur ulang, pengolahan limbah, dan pengurangan sampah.

- Transportasi Ramah Lingkungan: Pengembangan infrastruktur dan kendaraan listrik, transportasi publik rendah emisi, dan jalur sepeda.

- Efisiensi Energi: Peningkatan efisiensi di sektor industri, bangunan, dan rumah tangga.

- Adaptasi dan Mitigasi Perubahan Iklim: Proyek yang membantu komunitas beradaptasi dengan dampak perubahan iklim atau mengurangi emisi gas rumah kaca.

# Komponen Utama Green Finance:

**Investasi Hijau:** Ini merujuk pada proyek-proyek konkret yang dirancang untuk memberikan dampak lingkungan positif, seperti mengurangi emisi, menghemat energi, mengelola sumber daya secara berkelanjutan, atau mengkonservasi keanekaragaman hayati.

**Instrumen Keuangan Hijau:** Meliputi berbagai produk dan layanan keuangan yang dirancang khusus untuk memfasilitasi investasi hijau:

**Green Bond:** Obligasi yang penerbitannya secara spesifik untuk membiayai proyek-proyek hijau.

**Green Loan:** Pinjaman yang ditujukan untuk proyek dengan manfaat lingkungan.
ESG Fund (Environmental, Social, Governance Fund): Dana investasi yang memilih aset berdasarkan kriteria lingkungan, sosial, dan tata kelola perusahaan yang baik.

# Manfaat Green Finance:
**Pengurangan Risiko Jangka Panjang:** Membantu memitigasi risiko finansial dan operasional yang timbul dari perubahan iklim dan degradasi lingkungan.

**Peningkatan Transparansi Lingkungan:** Mendorong sektor keuangan untuk lebih transparan dalam pelaporan dampak lingkungan dari investasi mereka.

**Insentif Investor dan Penerbit:** Memberikan daya tarik bagi investor yang peduli lingkungan, seringkali melalui kondisi yang lebih menguntungkan (misalnya greenium, yaitu selisih imbal hasil yang lebih rendah pada green bond dibandingkan obligasi konvensional, menunjukkan permintaan yang tinggi).

# ⚖️ Regulasi Green Finance di Indonesia
Indonesia telah menunjukkan komitmen kuat terhadap keberlanjutan melalui pengembangan kerangka regulasi Green Finance yang progresif. Regulasi ini menjadi landasan bagi lembaga keuangan dan pelaku usaha untuk berinvestasi pada proyek-proyek hijau:

**1. Taksonomi Hijau Indonesia (THI) – OJK 2022:**

- Merupakan sistem klasifikasi komprehensif yang dikembangkan oleh Otoritas Jasa Keuangan (OJK) untuk menilai apakah sebuah kegiatan ekonomi tergolong "hijau" atau berkelanjutan.

- THI menetapkan kriteria teknis dan sektor prioritas yang jelas, memberikan panduan bagi investor dan lembaga keuangan dalam mengidentifikasi dan membiayai proyek yang benar-benar memberikan manfaat lingkungan.

**2. POJK No. 60/POJK.04/2017 tentang Penerbitan dan Persyaratan Efek Bersifat Utang dan Sukuk Berlandaskan Prinsip Syariah (Green Bond):**

- Peraturan ini secara khusus mengatur penerbitan Green Bond di Indonesia.

- Mencakup ketentuan mengenai pelaporan dampak lingkungan dari proyek yang dibiayai oleh Green Bond, serta penilaian kelayakan proyek hijau untuk memastikan integritas dan akuntabilitas.

**3. POJK No. 51/POJK.03/2017 tentang Penerapan Keuangan Berkelanjutan bagi Lembaga Jasa Keuangan, Emiten, dan Perusahaan Publik:**

- Mewajibkan lembaga keuangan untuk menyusun Rencana Aksi Keuangan Berkelanjutan (RAKB).

- Mendorong penilaian portofolio berdasarkan prinsip keberlanjutan, termasuk analisis Green Net Present Value (GNPV) dan dampak lingkungan, sosial, dan tata kelola (ESG), yang mendorong integrasi faktor-faktor non-finansial dalam pengambilan keputusan investasi.

# 2. Analisis Field Dataset
Bagian ini akan menjelaskan setiap dataset yang digunakan dalam analisis, beserta rumus dan temuan kunci dari setiap pertanyaan tugas. Kode Python yang digunakan untuk menghasilkan analisis juga akan disertakan.

**2.1 Financial Dataset**
Dataset ini krusial untuk menganalisis kelayakan ekonomi dan risiko finansial dari setiap proyek. Ini berisi informasi langsung terkait investasi dan pembiayaan.

**📊 Struktur Dataset**
---
|Nama Field|Deskripsi Singkat|
|---|---|
|Investment_Cost|Total dana yang diinvestasikan dalam proyek (dalam miliar rupiah). Ini adalah skala finansial proyek.|
|Loan_Interest_Rate|Suku bunga tahunan (%) yang diterapkan pada pinjaman proyek, memengaruhi biaya modal.|
|Default_Risk_Score|Skor risiko gagal bayar (0–100), menunjukkan probabilitas proyek tidak dapat memenuhi kewajiban finansialnya.|
|Green_Bond_Spread|Selisih imbal hasil (dalam basis poin, bps) antara green bond proyek ini dan obligasi biasa, mencerminkan greenium atau diskon/premium hijau.|
---


📐 Rumus Green Net Present Value (GNPV)

GNPV adalah metrik penting yang memperhitungkan tidak hanya arus kas finansial, tetapi juga nilai moneter dari eksternalitas lingkungan (misalnya, penghematan karbon).

GNPV= 
t=1
∑
N
​
  
(1+r) 
t
 
(CF 
t
​
 +E 
t
​
 )
​
 −I 
0
​
 
Keterangan:

textGNPV: Green Net Present Value (nilai kini bersih hijau).

textCF_t: Arus kas bersih konvensional pada tahun ke-t.

textE_t: Nilai eksternalitas lingkungan (misalnya pengurangan emisi CO₂, penghematan air) pada tahun ke-t.

r: Tingkat diskonto (contoh: 0.05 untuk 5%), merepresentasikan biaya modal atau return yang disyaratkan.

t: Tahun ke-t (periode waktu).

N: Umur proyek (dalam tahun).

textI_0: Investasi awal proyek.

✅ GNPV yang lebih tinggi menunjukkan proyek lebih layak secara finansial dan berkontribusi pada keberlanjutan lingkungan. Proyek dianggap layak jika 
textGNPV0.

Analisis GNPV dari data Financial_Dataset menunjukkan hasil sebagai berikut:

Kesimpulan Hasil: Proyek dengan GNPV positif secara konsisten dianggap layak menurut kaidah evaluasi finansial dan dampak lingkungan, mengindikasikan bahwa investasi tersebut menguntungkan secara ekonomi sambil memberikan manfaat lingkungan.

Dalam visualisasi, mayoritas proyek PLTS seperti PLTS-JABW-001, PLTS-JATIM-001, dan PLTS-NTB-001 menunjukkan GNPV tinggi, menandakan kombinasi arus kas yang kuat dan dampak lingkungan yang menguntungkan. Hal ini menunjukkan bahwa proyek tenaga surya seringkali memiliki kelayakan finansial yang tinggi di bawah skema Green Finance.

Beberapa PLTM juga menunjukkan kinerja baik, namun umumnya GNPV-nya lebih rendah dibandingkan PLTS, mungkin karena skala proyek yang lebih kecil atau efisiensi pengembalian lingkungan/finansial yang berbeda.

2.2 Environmental Dataset
Environmental Dataset adalah kumpulan data vital yang merekam dampak lingkungan yang dihasilkan oleh setiap proyek energi hijau. Dataset ini sangat penting dalam mendukung keputusan investasi berbasis lingkungan (green investment), khususnya dalam rangka transisi energi bersih dan kebijakan pembiayaan hijau di Indonesia.

📊 Struktur Dataset

Nama Kolom

Deskripsi Singkat

Project_ID

Kode unik untuk mengidentifikasi setiap proyek (misal: PLTS-NTT-001).

CO2_Reduction

Estimasi pengurangan emisi karbon tahunan (dalam ton CO2e), metrik kunci untuk dampak iklim.

Energy_Output

Produksi energi tahunan (dalam satuan kWh atau MWh), menunjukkan kontribusi proyek terhadap pasokan energi.

Environmental_Risk_Index

Skor risiko lingkungan proyek (skala 0–100, makin tinggi skornya, makin berisiko). Ini mencakup risiko seperti dampak terhadap ekosistem lokal.

Konteks_Lingkungan

Deskripsi singkat kondisi lingkungan atau ekologi setempat, memberikan konteks geografis dan ekologis.

Peringkat_Dampak

Penilaian kualitatif terhadap dampak lingkungan secara keseluruhan (contoh: High / Medium / Low).


Ekspor ke Spreadsheet
🌿 Rumus Carbon Return on Investment (CROI)

CROI adalah metrik efisiensi yang mengukur seberapa efektif investasi dalam proyek lingkungan dalam menghasilkan pengurangan emisi karbon. Semakin tinggi CROI, semakin banyak karbon yang dikurangi per unit investasi.

CROI= 
I 
0
​
 
∑ 
t=1
N
​
 (R 
t
​
 ×P 
C
​
 )
​
 
Keterangan:

textCROI: Carbon Return on Investment.

textR_t: Emisi karbon yang berhasil dikurangi pada tahun ke-t (ton CO₂e).

textP_C: Harga karbon per ton CO₂e (dalam Rupiah), merepresentasikan nilai moneter dari pengurangan emisi.

textI_0: Investasi awal proyek (dalam Rupiah).

N: Umur proyek (dalam tahun).

✅ Nilai CROI yang lebih tinggi menandakan efisiensi karbon yang lebih baik per unit investasi.

Pengerjaan Soal 1: Conditional Statements (If-Else) and Arithmetic Operations
Deskripsi: Pemerintah ingin mengidentifikasi proyek PLTS dengan efisiensi pengurangan CO2 yang tinggi per unit investasi, dihitung sebagai pengurangan CO2 per juta rupiah.

Pendekatan Analisis:

Untuk menjawab pertanyaan ini, kami menggabungkan data lingkungan dan finansial untuk mendapatkan gambaran komprehensif. Kemudian, kami menyaring proyek berdasarkan Project_ID yang dimulai dengan "PLTS" dan menghitung rasio efisiensi. Rasio ini dikategorikan sebagai "High" atau "Low" menggunakan logika kondisional.

Langkah-langkah Teknis:

Penggabungan Dataset: Menggunakan fungsi pd.merge() untuk menggabungkan df_environmental dan df_financial berdasarkan kolom Project_ID. Metode inner join digunakan untuk memastikan hanya proyek yang ada di kedua dataset yang dianalisis.

Penyaringan Data: Memfilter DataFrame yang telah digabungkan untuk hanya menyertakan baris di mana Project_ID dimulai dengan string "PLTS" menggunakan metode string .str.startswith().

Perhitungan Rasio Efisiensi: Rasio dihitung dengan membagi CO2_Reduction (dalam ton CO2e) dengan Investment_Cost (yang dikonversi dari miliar rupiah menjadi juta rupiah dengan mengalikan 1000). Penanganan ZeroDivisionError diimplementasikan untuk kasus di mana Investment_Cost adalah nol, mengembalikan NaN dan kemudian menampilkannya sebagai "Tidak dapat dihitung".

Klasifikasi Kondisional: Fungsi apply() dengan lambda expression digunakan untuk membuat kolom Category. Jika Ratio 
ge0.5, kategori adalah "High"; jika tidak, kategori adalah "Low". Penanganan NaN juga disertakan untuk rasio yang tidak dapat dihitung.

Pencetakan Hasil: Melakukan iterasi melalui baris DataFrame yang difilter dan mencetak Project_ID, Ratio (diformat dua desimal), dan Category menggunakan f-strings untuk output yang jelas dan mudah dibaca.

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 1: Conditional Statements (If-Else) and Arithmetic Operations ---
print("\n--- SOAL 1: Efisiensi Pengurangan CO2 Proyek PLTS ---")
print("Tujuan: Mengidentifikasi proyek PLTS dengan efisiensi pengurangan CO2 tinggi per juta rupiah investasi.\n")

# 1. Gabungkan Environmental_Dataset dan Financial_Dataset menggunakan Project_ID.
merged_df_q1 = pd.merge(df_environmental, df_financial, on='Project_ID', how='inner')

# 2. Untuk PLTS projects (Project_ID starts with "PLTS"), compute the ratio: CO2_Reduction / (Investment_Cost * 1_000_000).
# Catatan: Investment_Cost dalam billion rupiah. Untuk rasio per juta rupiah, kita kalikan 1_000 (karena 1 miliar = 1000 juta).
plts_projects = merged_df_q1[merged_df_q1['Project_ID'].str.startswith('PLTS')].copy()

# Hitung rasio, pastikan Investment_Cost tidak nol untuk menghindari ZeroDivisionError
plts_projects['Ratio'] = plts_projects.apply(
    lambda row: row['CO2_Reduction'] / (row['Investment_Cost'] * 1000) if row['Investment_Cost'] != 0 else np.nan,
    axis=1
)

# 3. Use if-else to classify the ratio as "High" (≥ 0.5 tons CO2e/million Rp) or "Low" (< 0.5).
plts_projects['Category'] = plts_projects['Ratio'].apply(lambda x: "High" if x >= 0.5 else "Low" if not pd.isna(x) else "N/A")

# 4. Display results as: "Project_ID: Ratio (Category)" using f-strings.
print("Output Hasil Analisis Soal 1:")
for index, row in plts_projects.iterrows():
    if not pd.isna(row['Ratio']):
        print(f"{row['Project_ID']}: {row['Ratio']:.2f} ({row['Category']})")
    else:
        print(f"{row['Project_ID']}: Tidak dapat dihitung (Biaya Investasi nol atau hilang)")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 1:

PLTS-NTT-001: 0.50 (High)
PLTS-JATIM-001: 0.45 (Low)
PLTS-SULSEL-001: 0.50 (High)
PLTS-JABW-001: 0.50 (High)
Interpretasi Hasil Soal 1:

Dari analisis ini, terlihat bahwa proyek-proyek PLTS seperti PLTS-NTT-001, PLTS-SULSEL-001, dan PLTS-JABW-001 menunjukkan efisiensi pengurangan CO2 yang tinggi (0.50 ton CO2e per juta rupiah investasi atau lebih). Ini berarti setiap satu juta rupiah yang diinvestasikan pada proyek-proyek ini menghasilkan pengurangan emisi CO2 yang signifikan, menjadikannya sangat menarik dari perspektif dampak lingkungan dan efisiensi investasi. Sebaliknya, proyek PLTS-JATIM-001 memiliki efisiensi yang sedikit lebih rendah (0.45), yang masih berkontribusi pada pengurangan CO2 tetapi tidak seefisien proyek kategori "High". Informasi ini krusial bagi pemerintah atau investor untuk mengarahkan pendanaan ke proyek-proyek yang menawarkan dampak lingkungan terbaik per unit investasi.

Pengerjaan Soal 2: For Loop and Lists
Deskripsi: Pemerintah perlu menghitung rata-rata pengurangan CO2 di seluruh proyek PLTM untuk menilai dampak lingkungan kolektif mereka.

Pendekatan Analisis:

Tugas ini berfokus pada penggunaan for loop dan lists untuk memproses data. Kami akan mengekstrak data pengurangan CO2 khusus untuk proyek PLTM, lalu menghitung total dan rata-rata secara manual menggunakan loop.

Langkah-langkah Teknis:

Ekstraksi Data: Melakukan iterasi melalui df_environmental. Setiap Project_ID diperiksa apakah dimulai dengan "PLTM" menggunakan .startswith(). Jika ya, nilai CO2_Reduction ditambahkan ke sebuah list bernama pltm_co2_reductions.

Agregasi Manual: Sebuah for loop terpisah digunakan untuk menjumlahkan semua nilai dalam pltm_co2_reductions dan menghitung jumlah proyek PLTM. Pendekatan ini secara eksplisit menunjukkan pemahaman tentang bagaimana for loop digunakan untuk agregasi.

Perhitungan Rata-rata: Rata-rata dihitung dengan membagi total pengurangan CO2 dengan jumlah proyek PLTM. Penanganan kasus di mana tidak ada proyek PLTM (untuk menghindari ZeroDivisionError) juga disertakan.

Pencetakan Hasil: Hasil rata-rata ditampilkan, dibulatkan ke bilangan bulat terdekat (.0f).

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 2: For Loop and Lists ---
print("\n--- SOAL 2: Rata-rata Pengurangan CO2 Proyek PLTM ---")
print("Tujuan: Menilai dampak lingkungan kolektif proyek PLTM dengan menghitung rata-rata pengurangan CO2 mereka.\n")

# 1. Gunakan Environmental_Dataset.xlsx. (df_environmental sudah dimuat di awal)

# 2. Buat list dari nilai CO2_Reduction untuk proyek PLTM (Project_ID starts with "PLTM").
pltm_co2_reductions = []
for index, row in df_environmental.iterrows():
    if row['Project_ID'].startswith('PLTM'):
        pltm_co2_reductions.append(row['CO2_Reduction'])

# 3. Gunakan for loop untuk menghitung total CO2 reduction dan jumlah proyek PLTM.
total_co2_reduction_pltm = 0
count_pltm_projects = 0

for co2_val in pltm_co2_reductions:
    total_co2_reduction_pltm += co2_val
    count_pltm_projects += 1

# 4. Hitung dan tampilkan rata-ratanya.
average_co2_reduction_pltm = 0
if count_pltm_projects > 0:
    average_co2_reduction_pltm = total_co2_reduction_pltm / count_pltm_projects
else:
    print("Tidak ada proyek PLTM yang ditemukan dalam dataset.")

print("Output Hasil Analisis Soal 2:")
print(f"Average CO2 Reduction for PLTM Projects: {average_co2_reduction_pltm:.0f} tons CO2e")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 2:

Average CO2 Reduction for PLTM Projects: 31500 tons CO2e
Interpretasi Hasil Soal 2:

Rata-rata pengurangan CO2 untuk proyek PLTM adalah 31,500 ton CO2e. Angka ini memberikan gambaran kolektif tentang kontribusi proyek-proyek PLTM terhadap mitigasi perubahan iklim. Meskipun mungkin lebih kecil dibandingkan proyek PLTS skala besar, kontribusi ini penting dalam portofolio energi terbarukan Indonesia, terutama karena PLTM sering beroperasi di lokasi terpencil dan dapat memberikan manfaat energi terdesentralisasi. Rata-rata ini menjadi metrik dasar untuk membandingkan kinerja lingkungan antar jenis proyek dan menginformasikan kebijakan di masa mendatang.

Pengerjaan Soal 3: While Loop and User Input
Deskripsi: Pemerintah membutuhkan alat untuk memeriksa status lahan dan tingkat konflik sosial dengan memasukkan Project_ID secara interaktif.

Pendekatan Analisis:

Soal ini menguji kemampuan dalam menangani input pengguna dan mengelola alur program menggunakan while loop. Sebuah dictionary digunakan untuk penyimpanan data yang efisien, memungkinkan pencarian data sosial proyek secara cepat.

Langkah-langkah Teknis:

Persiapan Data: df_social dikonversi menjadi sebuah dictionary (social_data_dict) di mana Project_ID menjadi kunci dan nilai adalah sebuah dictionary yang berisi kolom-kolom lain untuk baris tersebut. Ini memungkinkan pencarian data yang sangat cepat berdasarkan Project_ID.

While Loop Interaktif: Sebuah while loop tak terbatas (while True) digunakan untuk terus meminta input Project_ID dari pengguna. Loop akan berhenti ketika pengguna mengetik "DONE".

Penanganan Input:

Input pengguna diproses (.strip().upper()) untuk menghilangkan spasi berlebih dan mengubahnya menjadi huruf kapital agar pencarian tidak case-sensitive.

Jika input adalah "DONE", loop dihentikan dengan break.

Jika Project_ID ditemukan dalam social_data_dict, informasi Land_Status dan Tingkat_Konflik ditampilkan.

Jika Project_ID tidak ditemukan, pesan "Project not found" ditampilkan.

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 3: While Loop and User Input ---
print("\n--- SOAL 3: Pemeriksa Status Lahan dan Tingkat Konflik Proyek ---")
print("Tujuan: Menyediakan alat interaktif untuk memeriksa status lahan dan tingkat konflik sosial proyek.\n")

# 1. Gunakan Social_Dataset.xlsx. (df_social sudah dimuat di awal)

# Buat dictionary untuk akses cepat data sosial
social_data_dict = df_social.set_index('Project_ID').to_dict('index')

print("Output Hasil Analisis Soal 3:")
print("Masukkan Project_ID untuk melihat detail (ketik 'DONE' untuk selesai):")
while True:
    project_id_input = input("Enter Project_ID: ").strip().upper()

    if project_id_input == "DONE":
        print("Selesai.")
        break
    elif project_id_input in social_data_dict:
        data = social_data_dict[project_id_input]
        print(f"{project_id_input} - Land Status: {data['Land_Status']}, Tingkat Konflik: {data['Tingkat_Konflik']}")
    else:
        print("Project not found")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 3 (Contoh Interaksi):

Output Hasil Analisis Soal 3:
Masukkan Project_ID untuk melihat detail (ketik 'DONE' untuk selesai):
Enter Project_ID: PLTS-NTT-001
PLTS-NTT-001 - Land Status: Adat, Tingkat Konflik: High
Enter Project_ID: INVALID-ID
Project not found
Enter Project_ID: PLTS-JATIM-001
PLTS-JATIM-001 - Land Status: Negara, Tingkat Konflik: Low
Enter Project_ID: DONE
Selesai.
Interpretasi Hasil Soal 3:

Alat interaktif ini memungkinkan pengguna untuk dengan cepat mencari informasi kritis mengenai status lahan dan tingkat konflik sosial dari setiap proyek. Misalnya, dengan memasukkan "PLTS-NTT-001", kita dapat segera melihat bahwa status lahannya adalah "Adat" dengan "Tingkat Konflik: High", yang mengindikasikan potensi tantangan dalam akuisisi lahan atau penerimaan komunitas. Sebaliknya, "PLTS-JATIM-001" menunjukkan "Land Status: Negara" dan "Tingkat Konflik: Low", yang mungkin berarti jalur proyek yang lebih mulus dari perspektif sosial. Kemampuan untuk secara instan mengakses data ini sangat berharga untuk penilaian risiko awal dan perencanaan strategi keterlibatan masyarakat.

Pengerjaan Soal 4: Dictionary and Conditional Filtering
Deskripsi: Pemerintah mencari proyek dengan daya tarik investasi tinggi dan tingkat konflik sosial rendah untuk meminimalkan risiko.

Pendekatan Analisis:

Soal ini menggabungkan penggunaan dictionary dan conditional filtering. Data dari dua dataset berbeda digabungkan, kemudian diproses ke dalam dictionary untuk mempermudah pemfilteran berdasarkan kriteria ganda.

Langkah-langkah Teknis:

Penggabungan Data: df_economic dan df_social digabungkan menggunakan pd.merge() berdasarkan Project_ID. Ini penting karena kriteria yang diinginkan tersebar di dua dataset tersebut (Daya_Tarik_Investasi dari ekonomi dan Tingkat_Konflik dari sosial).

Pembentukan Dictionary: Sebuah dictionary baru (project_criteria_dict) dibuat. Setiap Project_ID dijadikan kunci, dan nilai yang terkait adalah sebuah tuple yang berisi Daya_Tarik_Investasi dan Tingkat_Konflik untuk proyek tersebut. Pendekatan ini mengkonsolidasi informasi yang relevan untuk setiap proyek.

Pemfilteran Kondisional: Sebuah for loop digunakan untuk mengiterasi melalui items() dari project_criteria_dict. Di dalam loop, pernyataan if digunakan untuk memeriksa dua kondisi secara bersamaan: Daya_Tarik_Investasi harus "High" DAN Tingkat_Konflik harus "Low". Proyek yang memenuhi kedua kriteria ini ditambahkan ke list filtered_projects_q4.

Pencetakan Hasil: Daftar Project_ID yang difilter dicetak. Jika tidak ada proyek yang memenuhi kriteria, pesan yang sesuai akan ditampilkan.

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 4: Dictionary and Conditional Filtering ---
print("\n--- SOAL 4: Proyek dengan Daya Tarik Investasi Tinggi dan Konflik Rendah ---")
print("Tujuan: Mengidentifikasi proyek yang optimal dengan daya tarik investasi tinggi dan risiko konflik sosial rendah.\n")

# 1. Gabungkan Economic_Dataset.xlsx dan Social_Dataset.xlsx menggunakan Project_ID.
merged_df_q4 = pd.merge(df_economic, df_social, on='Project_ID', how='inner')

# 2. Buat dictionary dengan Project_ID sebagai keys dan tuple (Daya_Tarik_Investasi, Tingkat_Konflik) sebagai values.
project_criteria_dict = {}
for index, row in merged_df_q4.iterrows():
    project_criteria_dict[row['Project_ID']] = (row['Daya_Tarik_Investasi'], row['Tingkat_Konflik'])

# 3. Gunakan for loop dengan if untuk memfilter proyek di mana Daya_Tarik_Investasi == "High" dan Tingkat_Konflik == "Low".
filtered_projects_q4 = []
for project_id, criteria in project_criteria_dict.items():
    if criteria[0] == "High" and criteria[1] == "Low":
        filtered_projects_q4.append(project_id)

# 4. Tampilkan Project_IDs yang difilter.
print("Output Hasil Analisis Soal 4:")
print("Projects with High Investment Attractiveness and Low Conflict:")
if filtered_projects_q4:
    for project_id in filtered_projects_q4:
        print(project_id)
else:
    print("Tidak ada proyek yang memenuhi kriteria ini dalam dataset.")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 4:

Projects with High Investment Attractiveness and Low Conflict:
PLTS-JATIM-001
PLTS-SULSEL-001
PLTS-JABW-001
Interpretasi Hasil Soal 4:

Analisis ini berhasil mengidentifikasi proyek-proyek yang paling menjanjikan dari sudut pandang ekonomi dan sosial. Proyek-proyek seperti PLTS-JATIM-001, PLTS-SULSEL-001, dan PLTS-JABW-001 memenuhi kriteria "Daya Tarik Investasi: High" dan "Tingkat Konflik: Low". Ini berarti proyek-proyek ini tidak hanya menarik secara finansial tetapi juga memiliki penerimaan komunitas yang baik dan risiko sosial yang minimal, menjadikannya pilihan investasi yang optimal bagi pemerintah yang ingin meminimalkan potensi hambatan dan memastikan keberlanjutan proyek dalam jangka panjang.

Pengerjaan Soal 5: Functions and Arithmetic
Deskripsi: Pemerintah perlu menghitung total investasi untuk proyek-proyek dengan efisiensi lokasi tinggi.

Pendekatan Analisis:

Soal ini menekankan penggunaan fungsi (def) untuk mengorganisir kode dan melakukan perhitungan aritmatika. Data lokasi dan finansial digabungkan, dan fungsi yang dibuat akan memproses data ini untuk menjumlahkan investasi dari proyek-proyek yang memenuhi kriteria lokasi.

Langkah-langkah Teknis:

Penggabungan Data: df_geospatial dan df_financial digabungkan berdasarkan Project_ID untuk mendapatkan informasi Efisiensi_Lokasi dan Investment_Cost dalam satu DataFrame.

Definisi Fungsi (calculate_total_investment):

Fungsi ini menerima satu argumen: sebuah DataFrame yang telah digabungkan.

Di dalamnya, sebuah for loop mengiterasi setiap baris DataFrame.

Kondisi if row['Efisiensi_Lokasi'] == "High" digunakan untuk memfilter proyek.

Jika kondisi terpenuhi, Investment_Cost dari proyek tersebut ditambahkan ke total_investment.

Fungsi mengembalikan total investasi.

Pemanggilan Fungsi dan Pencetakan Hasil: Fungsi calculate_total_investment dipanggil dengan DataFrame gabungan sebagai argumen. Hasilnya kemudian dicetak dengan format yang rapi, dibulatkan hingga dua desimal, dan diberi satuan "billion Rp".

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 5: Functions and Arithmetic ---
print("\n--- SOAL 5: Total Investasi untuk Lokasi Efisiensi Tinggi ---")
print("Tujuan: Menghitung akumulasi investasi pada proyek-proyek yang berlokasi sangat efisien.\n")

# 1. Gabungkan Geospatial_Dataset.xlsx dan Financial_Dataset.xlsx.
merged_df_q5 = pd.merge(df_geospatial, df_financial, on='Project_ID', how='inner')

# 2. Definisikan fungsi calculate_total_investment.
def calculate_total_investment(data_frame):
    """
    Menghitung total Investment_Cost untuk proyek dengan Efisiensi_Lokasi "High".

    Args:
        data_frame (pd.DataFrame): DataFrame gabungan dari data Geospatial dan Financial.

    Returns:
        float: Total Investment_Cost dalam billion Rp.
    """
    total_investment = 0
    for index, row in data_frame.iterrows():
        if row['Efisiensi_Lokasi'] == "High":
            total_investment += row['Investment_Cost']
    return total_investment

# 3. Panggil fungsi dan tampilkan hasilnya.
total_inv_high_efficiency = calculate_total_investment(merged_df_q5)

print("Output Hasil Analisis Soal 5:")
print(f"Total Investment for High-Efficiency Locations: {total_inv_high_efficiency:.2f} billion Rp")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 5:

Total Investment for High-Efficiency Locations: 330.00 billion Rp
Interpretasi Hasil Soal 5:

Analisis ini menunjukkan bahwa total investasi untuk proyek-proyek yang berlokasi dengan efisiensi tinggi adalah 330.00 miliar Rp. Angka ini sangat penting untuk pengalokasian sumber daya. Lokasi dengan efisiensi tinggi (misalnya, karena iradiasi surya optimal, kedekatan dengan jaringan listrik, atau aksesibilitas yang baik) seringkali menawarkan potensi pengembalian investasi yang lebih besar dan risiko operasional yang lebih rendah. Oleh karena itu, mengetahui total investasi di area-area ini membantu pemerintah dan investor dalam mengidentifikasi seberapa besar modal yang telah diarahkan ke proyek-proyek dengan potensi keberhasilan yang lebih tinggi.

Pengerjaan Soal 6: Modules and Error Handling
Deskripsi: Pemerintah memerlukan alat yang dapat digunakan kembali untuk menghitung efisiensi pengurangan CO2 dengan penanganan kesalahan.

Pendekatan Analisis:

Soal ini berfokus pada modularitas dan penanganan kesalahan (try-except). Sebuah fungsi untuk menghitung efisiensi CO2 dibuat dalam modul terpisah (green_analysis.py), dan kemudian diimpor serta diuji di skrip utama. Penanganan kesalahan diterapkan untuk kasus ZeroDivisionError dan tipe input yang tidak valid.

Langkah-langkah Teknis:

Pembuatan Modul: File green_analysis.py dibuat (seperti yang sudah kita siapkan), berisi fungsi compute_co2_efficiency. Fungsi ini menghitung rasio CO2_Reduction terhadap Investment_Cost (dikonversi ke juta rupiah).

Penanganan Kesalahan dalam Modul:

try-except ZeroDivisionError: Blok try-except digunakan untuk menangkap kondisi di mana Investment_Cost adalah nol setelah dikonversi ke juta rupiah, mengembalikan pesan "Cannot compute: Investment Cost is zero."

try-except ValueError: Ditambahkan untuk menangani kasus di mana CO2_Reduction atau Investment_Cost bukan angka, mengembalikan pesan "Cannot compute: Invalid input types (non-numeric)."

try-except Exception: Sebagai penanganan umum untuk error lain yang tidak terduga.

Import Modul: Di main_analysis.py, fungsi compute_co2_efficiency diimpor dari green_analysis.py. Penanganan ImportError juga ditambahkan jika modul tidak dapat ditemukan.

Pengujian Fungsi: Fungsi ini diuji pada beberapa data proyek contoh, termasuk skenario di mana Investment_Cost adalah nol dan input adalah tipe yang salah, untuk menunjukkan bahwa penanganan kesalahan bekerja dengan baik.

Kode Python (dalam green_analysis.py):

Python

# green_analysis.py

def compute_co2_efficiency(co2_reduction, investment_cost_billion_rp):
    """
    Menghitung efisiensi pengurangan CO2 per juta rupiah investasi.

    Args:
        co2_reduction (float/int): Pengurangan CO2 dalam ton CO2e.
        investment_cost_billion_rp (float/int): Biaya investasi dalam miliar rupiah.

    Returns:
        float or str: Rasio efisiensi atau pesan error jika Investment_Cost adalah 0 atau tipe data salah.
    """
    try:
        # Pastikan input adalah angka yang dapat dikonversi
        co2_reduction = float(co2_reduction)
        investment_cost_billion_rp = float(investment_cost_billion_rp)

        # Konversi billion rupiah ke million rupiah
        investment_cost_million_rp = investment_cost_billion_rp * 1_000
        if investment_cost_million_rp == 0:
            raise ZeroDivisionError("Investment Cost (in million Rp) is zero.")
        ratio = co2_reduction / investment_cost_million_rp
        return ratio
    except ZeroDivisionError:
        return "Cannot compute: Investment Cost is zero."
    except ValueError: # Menangani jika konversi ke float gagal (misal input string non-numeric)
        return "Cannot compute: Invalid input types (non-numeric)."
    except Exception as e: # Tangani error lain yang tidak terduga
        return f"An unexpected error occurred: {e}"

Kode Python (tambahan di main_analysis.py):

Python

# --- SOAL 6: Modules and Error Handling ---
print("\n--- SOAL 6: Komputasi Efisiensi Pengurangan CO2 dengan Error Handling ---")
print("Tujuan: Membuat alat yang dapat digunakan kembali dan tangguh untuk menghitung efisiensi CO2, dengan penanganan kesalahan yang robust.\n")

# Impor modul green_analysis yang sudah dibuat
try:
    from green_analysis import compute_co2_efficiency
    print("Modul 'green_analysis.py' berhasil diimpor.")
except ImportError:
    print("Error: Pastikan file 'green_analysis.py' berada di direktori yang sama dengan script ini.")
    print("Soal 6 akan dilewati karena modul tidak dapat diimpor.")
    compute_co2_efficiency = None # Set to None so subsequent calls don't fail

if compute_co2_efficiency: # Jalankan hanya jika modul berhasil diimpor
    # Data proyek untuk pengujian, termasuk skenario error
    test_projects = [
        {'Project_ID': 'PLTS-NTT-001', 'CO2_Reduction': 50000, 'Investment_Cost': 100}, # Ratio: 0.50
        {'Project_ID': 'PLTS-JATIM-001', 'CO2_Reduction': 45000, 'Investment_Cost': 100}, # Ratio: 0.45
        {'Project_ID': 'PLTM-PAPU-001', 'CO2_Reduction': 35000, 'Investment_Cost': 80},  # Ratio: 0.44
        {'Project_ID': 'TEST-ZERO-INV', 'CO2_Reduction': 10000, 'Investment_Cost': 0}, # Test ZeroDivisionError
        {'Project_ID': 'TEST-INVALID-TYPE', 'CO2_Reduction': 'abc', 'Investment_Cost': 50} # Test ValueError
    ]

    print("Output Hasil Analisis Soal 6:")
    for project in test_projects:
        co2_red = project['CO2_Reduction']
        inv_cost = project['Investment_Cost']
        efficiency = compute_co2_efficiency(co2_red, inv_cost)

        if isinstance(efficiency, (float, int)):
            print(f"{project['Project_ID']}: {efficiency:.2f}")
        else:
            print(f"{project['Project_ID']}: {efficiency}")
else:
    print("Soal 6 tidak dapat dijalankan.")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 6:

Modul 'green_analysis.py' berhasil diimpor.
Output Hasil Analisis Soal 6:
PLTS-NTT-001: 0.50
PLTS-JATIM-001: 0.45
PLTM-PAPU-001: 0.44
TEST-ZERO-INV: Cannot compute: Investment Cost is zero.
TEST-INVALID-TYPE: Cannot compute: Invalid input types (non-numeric).
Interpretasi Hasil Soal 6:

Fungsi compute_co2_efficiency yang dibuat dalam modul terpisah menunjukkan modularitas yang baik, memungkinkan fungsi ini digunakan kembali di berbagai bagian kode atau proyek lain. Yang lebih penting, fungsi ini menunjukkan robustness melalui penanganan kesalahan yang efektif. Saat diuji dengan data normal (PLTS-NTT-001, PLTS-JATIM-001, PLTM-PAPU-001), ia memberikan hasil efisiensi yang akurat. Namun, ketika menghadapi Investment_Cost nol (TEST-ZERO-INV) atau tipe data yang tidak valid (TEST-INVALID-TYPE), fungsi tersebut tidak crash melainkan mengembalikan pesan kesalahan yang informatif. Ini krusial dalam aplikasi dunia nyata di mana data seringkali tidak sempurna, memastikan program tetap berjalan stabil.

Pengerjaan Soal 7: Error Handling in Loops
Deskripsi: Pemerintah perlu menghitung rata-rata energi output dari proyek terpilih, dengan menangani data yang mungkin hilang.

Pendekatan Analisis:

Soal ini menekankan penanganan kesalahan dalam konteks loop saat memproses data. Hal ini sering terjadi dalam analisis data nyata di mana tidak semua data mungkin tersedia untuk setiap entri. try-except digunakan di dalam loop untuk mengelola KeyError yang terjadi ketika Project_ID tidak ditemukan.

Langkah-langkah Teknis:

Daftar Proyek Target: Sebuah list projects_to_analyze dibuat yang berisi Project_ID yang ingin dianalisis, termasuk satu ID yang sengaja tidak ada dalam dataset (PROJECT-NONEXISTENT) untuk menguji penanganan kesalahan.

Persiapan Data untuk Pencarian Cepat: Energy_Output dari df_environmental dikonversi menjadi sebuah dictionary (energy_output_dict) dengan Project_ID sebagai kunci. Ini memungkinkan pencarian Energy_Output yang sangat cepat.

Loop dengan try-except:

Sebuah for loop mengiterasi melalui setiap Project_ID dalam projects_to_analyze.

Di dalam loop, sebuah blok try mencoba untuk mengakses energy_output_dict menggunakan Project_ID saat ini.

Jika Project_ID tidak ditemukan (menyebabkan KeyError), blok except KeyError akan menangkap kesalahan tersebut dan mencetak pesan peringatan yang relevan tanpa menghentikan eksekusi loop.

Jika Project_ID ditemukan, Energy_Output ditambahkan ke total_energy_output dan valid_project_count bertambah.

Sebuah except Exception generik ditambahkan untuk menangani error lain yang tidak terduga.

Perhitungan Rata-rata: Setelah loop selesai, rata-rata Energy_Output dihitung berdasarkan total output dan jumlah proyek yang valid. Penanganan pembagian dengan nol juga disertakan.

Kode Python (dalam main_analysis.py):

Python

# --- SOAL 7: Error Handling in Loops ---
print("\n--- SOAL 7: Rata-rata Energi Output Proyek Terpilih dengan Penanganan Data Hilang ---")
print("Tujuan: Menghitung rata-rata energi output proyek yang dipilih, dengan gracefully menangani data yang hilang.\n")

# 1. Buat list dari Project_IDs untuk dianalisis.
projects_to_analyze = ['PLTS-NTT-001', 'PLTM-PAPU-001', 'PROJECT-NONEXISTENT', 'PLTS-JATIM-001', 'PLTS-SULSEL-001']

# Siapkan dictionary untuk pencarian cepat Energy_Output
energy_output_dict = df_environmental.set_index('Project_ID')['Energy_Output'].to_dict()

total_energy_output = 0
valid_project_count = 0

print("Output Hasil Analisis Soal 7:")
# 2. Gunakan for loop dengan try-except untuk memproses Energy_Output.
for project_id in projects_to_analyze:
    try:
        energy = energy_output_dict[project_id]
        total_energy_output += energy
        valid_project_count += 1
        print(f"Processing {project_id}: Energy Output = {energy} kWh")
    except KeyError:
        print(f"Warning: Project_ID '{project_id}' not found in Environmental Dataset. Skipping.")
    except Exception as e: # Tangani error lain yang mungkin terjadi
        print(f"An unexpected error occurred for {project_id}: {e}")

# 3. Hitung dan tampilkan rata-rata.
average_energy_output = 0
if valid_project_count > 0:
    average_energy_output = total_energy_output / valid_project_count
else:
    print("\nTidak ada proyek valid yang ditemukan untuk dihitung rata-rata Energy Output.")

print(f"\nAverage Energy Output: {average_energy_output:.0f} kWh")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Soal 7:

Output Hasil Analisis Soal 7:
Processing PLTS-NTT-001: Energy Output = 10000 kWh
Processing PLTM-PAPU-001: Energy Output = 7000 kWh
Warning: Project_ID 'PROJECT-NONEXISTENT' not found in Environmental Dataset. Skipping.
Processing PLTS-JATIM-001: Energy Output = 8000 kWh
Processing PLTS-SULSEL-001: Energy Output = 12000 kWh

Average Energy Output: 9250 kWh
Interpretasi Hasil Soal 7:

Soal ini secara efektif menunjukkan pentingnya penanganan kesalahan dalam loop untuk menjaga kelancaran analisis data. Meskipun PROJECT-NONEXISTENT tidak ditemukan dalam dataset, program tidak berhenti (crash) melainkan memberikan peringatan dan melanjutkan pemrosesan proyek-proyek yang valid. Hasilnya menunjukkan rata-rata Energy Output sebesar 9250 kWh dari proyek-proyek yang berhasil ditemukan. Ini adalah demonstrasi yang sangat baik tentang bagaimana kode yang tangguh dapat memproses dataset yang tidak lengkap atau 'kotor' tanpa menghentikan alur kerja, memastikan bahwa metrik penting seperti rata-rata output energi masih dapat dihitung bahkan dengan adanya data yang hilang.

Bonus Question: Machine Learning/AI with Decision Tree
Deskripsi: Pemerintah bertujuan untuk memprediksi daya tarik investasi ("High", "Medium", "Low") untuk proyek-proyek baru berdasarkan fitur-fitur seperti GDP_Growth, CO2_Reduction, dan Investment_Cost.

Pendekatan Analisis:

Soal bonus ini memperkenalkan konsep Machine Learning, khususnya Decision Tree Classifier, untuk memprediksi kategori target berdasarkan fitur numerik. Ini melibatkan penggabungan data, persiapan fitur, pemisahan data, pelatihan model, evaluasi, dan prediksi.

Langkah-langkah Teknis:

Penggabungan Data: Dataset Economic_Dataset, Environmental_Dataset, dan Financial_Dataset digabungkan secara berurutan menggunakan pd.merge() untuk mengumpulkan semua fitur dan target yang diperlukan dalam satu DataFrame.

Pemilihan Fitur dan Target: Kolom GDP_Growth, CO2_Reduction, dan Investment_Cost dipilih sebagai fitur (X), dan Daya_Tarik_Investasi dipilih sebagai variabel target (y).

Persiapan Data: Baris dengan nilai yang hilang (NaN) dalam kolom fitur atau target dihapus untuk memastikan model menerima input yang bersih.

Pemisahan Data: Data dibagi menjadi training set (80%) dan testing set (20%) menggunakan train_test_split dari scikit-learn. random_state=42 digunakan untuk memastikan hasil yang dapat direproduksi, dan stratify=y digunakan untuk menjaga proporsi kelas target yang sama di set pelatihan dan pengujian (jika memungkinkan).

Pelatihan Model: Sebuah DecisionTreeClassifier diinisialisasi dan dilatih (fit()) menggunakan training data.

Evaluasi Model: Model digunakan untuk membuat prediksi pada testing set (predict(X_test)). Akurasi model diukur menggunakan accuracy_score yang membandingkan prediksi dengan nilai y_test yang sebenarnya.

Prediksi Proyek Baru: Data untuk proyek baru dibuat dalam format DataFrame yang sesuai dengan fitur yang digunakan model. Model kemudian digunakan untuk memprediksi Daya_Tarik_Investasi untuk proyek baru ini.

Konsep dan Metode:

Decision Tree Classifier: Model Machine Learning yang membagi data menjadi "cabang-cabang" berdasarkan nilai fitur untuk mengklasifikasikan hasil. Ini membangun serangkaian aturan if-else dari data.

Data Preparation: Menggabungkan dan membersihkan data, memilih kolom yang relevan sebagai fitur (X) dan variabel yang akan diprediksi (y).

Splitting Data (train_test_split): Memisahkan dataset menjadi dua bagian: satu untuk melatih model (agar model belajar pola) dan satu lagi untuk menguji seberapa baik model dapat menggeneralisasi ke data baru yang belum pernah dilihatnya.

Training (.fit()): Proses di mana model belajar pola dari training data.

Evaluation (accuracy_score): Mengukur seberapa sering prediksi model cocok dengan nilai sebenarnya di testing set.

Prediction (.predict()): Menggunakan model yang sudah dilatih untuk memperkirakan output untuk data baru.

Kode Python (tambahan di main_analysis.py):

Python

# --- BONUS QUESTION: Machine Learning/AI with Decision Tree ---
print("\n--- BONUS QUESTION: Prediksi Daya Tarik Investasi dengan Decision Tree ---")
print("Tujuan: Memprediksi daya tarik investasi proyek baru menggunakan model Decision Tree Classifier.\n")

# Import scikit-learn libraries for the bonus question
from sklearn.tree import DecisionTreeClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

# 1. Merge Economic_Dataset.xlsx, Environmental_Dataset.xlsx, and Financial_Dataset.xlsx.
merged_df_bonus = pd.merge(df_economic, df_environmental, on='Project_ID', how='inner')
merged_df_bonus = pd.merge(merged_df_bonus, df_financial, on='Project_ID', how='inner')

# 2. Use scikit-learn to build a Decision Tree Classifier with Daya_Tarik_Investasi as the target.
# Select features and target
features = ['GDP_Growth', 'CO2_Reduction', 'Investment_Cost']
target = 'Daya_Tarik_Investasi'

# Prepare data: Drop rows with any NaN values in features or target for simplicity
model_data = merged_df_bonus.dropna(subset=features + [target])

X = model_data[features]
y = model_data[target]

# Splitting data into training (80%) and testing (20%) sets.
# Use stratify=y to ensure proportional representation of target classes if possible
try:
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42, stratify=y)
except ValueError:
    # Fallback if stratify is not possible (e.g., only one class in y, or too few samples)
    print("Warning: stratify not possible due to limited classes/samples, proceeding without it.")
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)


# Training the model
dt_classifier = DecisionTreeClassifier(random_state=42)
dt_classifier.fit(X_train, y_train)

# Evaluating accuracy
y_pred = dt_classifier.predict(X_test)
model_accuracy = accuracy_score(y_test, y_pred)

# Predicting for a new project
# Example new project data (GDP_Growth=5.0, CO2_Reduction=70000, Investment_Cost=150)
new_project_data = pd.DataFrame([[5.0, 70000, 150]], columns=features)
prediction = dt_classifier.predict(new_project_data)

print("Output Hasil Analisis Bonus Question:")
print(f"Model Accuracy: {model_accuracy:.2f}")
print(f"Prediction for new project (GDP_Growth=5.0, CO2_Reduction=70000, Investment_Cost=150): {prediction[0]}")

print("\n" + "-" * 80 + "\n")
Output Hasil Analisis Bonus Question:

Output Hasil Analisis Bonus Question:
Warning: stratify not possible due to limited classes/samples, proceeding without it.
Model Accuracy: 1.00
Prediction for new project (GDP_Growth=5.0, CO2_Reduction=70000, Investment_Cost=150): High
Interpretasi Hasil Bonus Question:

Model Decision Tree Classifier yang dilatih menunjukkan akurasi 1.00 pada data uji. Ini berarti model mampu memprediksi Daya_Tarik_Investasi dengan sempurna untuk data yang telah dilihatnya (dalam set pengujian). Akurasi setinggi ini pada dataset dummy yang kecil mungkin menunjukkan overfitting atau data yang terlalu sederhana, tetapi ini adalah demonstrasi yang baik dari konsepnya.

Ketika model digunakan untuk memprediksi proyek baru dengan GDP_Growth=5.0, CO2_Reduction=70000, dan Investment_Cost=150, prediksinya adalah "High". Ini menunjukkan bahwa berdasarkan pola yang dipelajari dari data historis, kombinasi fitur-fitur ini mengindikasikan daya tarik investasi yang kuat. Penerapan model ML semacam ini dapat sangat membantu pemerintah atau investor dalam menyaring dan memprioritaskan proyek-proyek hijau yang paling menjanjikan, mengurangi risiko dan mengoptimalkan alokasi dana.

2.3 Social Dataset
Social Dataset adalah data yang digunakan untuk mengukur dampak proyek terhadap masyarakat, sebuah aspek krusial dalam kerangka ESG (Environmental, Social, and Governance). Analisis data ini membantu menilai apakah proyek memberikan manfaat berkelanjutan dan inklusif bagi masyarakat lokal.

📊 Struktur Dataset

Nama Field

Deskripsi Singkat

Jobs_Created

Jumlah pekerjaan Full-Time Equivalent (FTE) yang dihasilkan proyek, mencerminkan manfaat ekonomi lokal.

Community_Engagement_Score

Tingkat penerimaan dan partisipasi masyarakat, dinilai dari skor 0–100.

Access_to_Clean_Energy_Rate

Persentase kenaikan akses masyarakat ke energi bersih, terutama wilayah 3T (Terdepan, Terluar, Tertinggal).

Gini_Coefficient_Impact

Efek proyek terhadap ketimpangan pendapatan; nilai negatif menunjukkan ketimpangan menurun.


Ekspor ke Spreadsheet
🤝 Rumus Social Return on Investment (SROI)

SROI adalah metrik untuk mengukur nilai sosial yang dihasilkan per unit investasi.

SROI= 
I 
0
​
 
NPV 
social
​
 
​
 
Keterangan:

textSROI: Social Return on Investment, menunjukkan berapa nilai sosial yang dihasilkan per rupiah investasi.

textNPV_textsocial: Nilai sekarang (Net Present Value) dari seluruh dampak sosial yang dimonetisasi (dalam rupiah).

textI_0: Investasi awal proyek (dalam rupiah).

Hasil analisis dari data Social_Dataset menunjukkan hasil sebagai berikut:
(Anda bisa menambahkan kesimpulan analisis SROI Anda di sini setelah melakukan perhitungannya)

2.4 Economic Dataset
Dataset ini memberikan gambaran kondisi ekonomi makro di wilayah atau negara tempat proyek dijalankan. Informasi ini penting untuk memahami risiko dan potensi keberhasilan proyek dari sisi ekonomi nasional, serta bagaimana proyek dapat berinteraksi dengan kondisi ekonomi yang lebih luas.

📊 Struktur Dataset

Nama Field

Deskripsi Singkat

GDP_Growth

Laju pertumbuhan ekonomi tahunan (dalam persen). Pertumbuhan tinggi berarti peluang pasar energi makin besar.

Inflation_Rate

Tingkat inflasi tahunan (dalam persen). Inflasi tinggi dapat menyebabkan biaya proyek naik.

FDI_Inflows

Masuknya investasi asing langsung (dalam miliar USD/IDR). Mencerminkan kepercayaan investor asing terhadap iklim usaha.

Unemployment_Rate

Persentase pengangguran. Tingkat pengangguran tinggi berarti proyek punya dampak sosial lebih besar dalam penciptaan lapangan kerja.


Ekspor ke Spreadsheet
📉 Rumus Economic Risk Adjustment Factor (ERAF)

ERAF adalah skor penyesuaian risiko ekonomi yang membantu mengevaluasi seberapa besar kondisi ekonomi makro dapat memengaruhi kelayakan proyek.

ERAF=w 
1
​
 ( 
IR 
base
​
 
IR 
t
​
 −IR 
base
​
 
​
 )+w 
2
​
 ( 
UR 
base
​
 
UR 
t
​
 −UR 
base
​
 
​
 )−w 
3
​
 ( 
GDP 
base
​
 
GDP 
t
​
 −GDP 
base
​
 
​
 )
Keterangan:

textERAF: Economic Risk Adjustment Factor, skor penyesuaian risiko ekonomi (tanpa satuan).

textIR_t: Tingkat inflasi saat ini (Inflation Rate).

textIR_textbase: Inflasi dasar atau target bank sentral.

textUR_t: Tingkat pengangguran saat ini.

textUR_textbase: Pengangguran dasar (rata-rata historis).

textGDP_t: Pertumbuhan Produk Domestik Bruto (PDB) saat ini.

textGDP_textbase: Pertumbuhan PDB dasar (rata-rata historis).

w_1,w_2,w_3: Bobot faktor risiko (jumlahnya = 1), ditentukan melalui metode seperti Analytic Hierarchy Process (AHP).

Dari analisis Economic_Dataset menunjukkan hasil sebagai berikut:
(Anda bisa menambahkan kesimpulan analisis ERAF Anda di sini setelah melakukan perhitungannya)

2.5 Geospatial Dataset
Dataset ini menyajikan data lokasi proyek yang penting untuk menilai risiko lingkungan dan keberlanjutan proyek dari sisi spasial. Faktor-faktor geografis dapat secara signifikan memengaruhi biaya, operasional, dan dampak lingkungan dari sebuah proyek.

📊 Struktur Dataset

Nama Field

Deskripsi Singkat

Latitude / Longitude

Titik koordinat lokasi proyek, esensial untuk analisis peta dan risiko alam.

Proximity_to_Protected_Area

Jarak (dalam km) ke kawasan lindung. Jarak yang dekat dapat meningkatkan potensi risiko regulasi dan lingkungan.

Land_Use_Change

Perubahan fungsi lahan akibat proyek (misalnya hutan menjadi perkebunan). Perubahan signifikan dapat meningkatkan risiko lingkungan dan sosial.

Efisiensi_Lokasi

Penilaian kualitatif efisiensi lokasi (High, Medium, Low), merefleksikan kesesuaian berdasarkan faktor seperti iradiasi surya atau kedekatan jaringan.


Ekspor ke Spreadsheet
🌍 Rumus Geospatial Risk Index (GRI)

GRI adalah skor risiko lokasi yang membantu menilai potensi ancaman lingkungan atau operasional yang terkait dengan geografi proyek.

GRI=w 
1
​
 ⋅H+w 
2
​
 ⋅P+w 
3
​
 ⋅L
Keterangan:

textGRI: Geospatial Risk Index, skor risiko lokasi (0–1).

textH: Skor risiko bencana alam, dinormalisasi dari data historis BNPB/BMKG (Badan Nasional Penanggulangan Bencana / Badan Meteorologi, Klimatologi, dan Geofisika).

textP: Skor risiko kedekatan dengan kawasan lindung, berasal dari Proximity_to_Protected_Area.

textL: Skor risiko perubahan tutupan lahan (Land_Use_Change).

w_1,w_2,w_3: Bobot faktor risiko (jumlahnya = 1), ditentukan melalui metode seperti Analytic Hierarchy Process (AHP), yang memungkinkan pembobotan prioritas risiko.

Aturan Praktis:

GRI mendekati 1 
rightarrow Risiko tinggi 
rightarrow perlu uji tuntas mendalam dan mitigasi risiko yang kuat.

Gunakan data spasial resmi (Ina-Geoportal, KLHK, BNPB) untuk akurasi yang lebih tinggi.

Dari analisis data Geospatial_Dataset menunjukkan hasil sebagai berikut:
(Anda bisa menambahkan kesimpulan analisis GRI Anda di sini setelah melakukan perhitungannya)

📌 Kesimpulan Umum
Analisis proyek Green Finance ini secara komprehensif menunjukkan bahwa keberlanjutan proyek energi hijau tidak hanya ditentukan oleh aspek finansial semata, tetapi juga oleh faktor lingkungan, sosial, ekonomi makro, dan risiko spasial. Integrasi berbagai dimensi ini memberikan gambaran yang jauh lebih akurat dan holistik tentang kelayakan dan dampak sebuah proyek.

💰 Financial Dataset memperlihatkan bahwa proyek dengan arus kas stabil dan investasi yang efisien cenderung lebih layak secara ekonomi, membentuk dasar keberhasilan finansial.

🌱 Environmental Dataset menegaskan pentingnya efisiensi emisi dan penghematan sumber daya sebagai indikator keberhasilan proyek hijau yang tidak bisa ditawar, mengukur dampak lingkungan yang nyata.

🧑‍🤝‍🧑 Social Dataset menyoroti kontribusi proyek terhadap penciptaan lapangan kerja, keterlibatan masyarakat yang positif, dan pengurangan ketimpangan, yang vital untuk keberlanjutan sosial.

📈 Economic Dataset memberi konteks penting dalam membaca dinamika risiko makro yang dapat memengaruhi kelayakan jangka panjang proyek, seperti inflasi dan pertumbuhan PDB.

🗺️ Geospatial Dataset membantu mengidentifikasi potensi risiko lokasi seperti bencana alam, kedekatan dengan kawasan lindung, dan perubahan tutupan lahan, memungkinkan perencanaan mitigasi yang proaktif.

Melalui integrasi kelima hal ini, pendekatan Green Finance mampu memberi pandangan yang lebih adil dan akurat dalam menilai proyek energi berkelanjutan, baik dari sisi dampak maupun risikonya. Analisis ini menjadi landasan kuat untuk pengambilan keputusan berbasis data yang tidak hanya menguntungkan secara finansial tetapi juga bertanggung jawab secara lingkungan dan sosial.

Terima kasih sudah membaca repository ini! Semoga analisis ini menginspirasi kita semua untuk membuat keputusan berbasis data yang lebih hijau dan berkeadilan. Sampai jumpa di repository berikutnya dan tetap semangat, Sobat ETL 🌿💡📊
