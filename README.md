# CasingJetsonOrinNano
Proses cara membuat casing pelindung untuk mini PC/development board seperti Jetson Orin Nano

# Pemodelan Mekanis: Desain & Assembly Casing Mini PC (SolidWorks)

Selamat datang di repository **Desain Casing Mini PC**. Repository ini mendokumentasikan proses perancangan dan perakitan (*assembly*) 3D casing pelindung untuk development board Jetson Orin Nano menggunakan *software* SolidWorks.
Proyek ini dibuat sebagai bagian dari Praktikum CAD CAM di program studi Teknologi Rekayasa Otomasi, bertujuan untuk melatih akurasi dimensi mekanis dan pemahaman struktur komponen modular.

## Tentang Proyek Ini
Dalam dunia otomasi dan IoT, perangkat keras seperti Raspberry Pi atau Jetson Orin Nano membutuhkan perlindungan fisik yang pas namun tetap fungsional (memiliki akses port dan ventilasi yang cukup). Proyek ini membedah bagaimana memanfaatkan fitur-fitur dasar SolidWorks untuk membangun sebuah casing fungsional dengan toleransi ukuran yang presisi.

## Alur Kerja Desain (Workflow)

### 1. Pemodelan Part Baru (*Part Modeling*)
Membuat geometri komponen pembentuk dari dasar sketsa 2D hingga menjadi objek 3D:
* **Fitur Sketsa:** Menggunakan *Rectangle Tool* untuk dimensi luar, *Circle Tool* untuk lubang baut & ventilasi, serta *Slot Tool* untuk akses kabel.
* **Fitur Pemodelan:** Menggunakan **Extruded Boss/Base** untuk memberikan ketebalan, **Extruded Cut** untuk melubangi port fisik (USB, HDMI, LAN), dan **Fillet** untuk menghaluskan sudut tajam.

### 2. Pengukuran Akurat (*Precision Dimensioning*)
* Penerapan ukuran berbasis milimeter (mm) menggunakan **Smart Dimension** yang disesuaikan dengan *datasheet* resmi papan sirkuit komputer.

### 3. Perakitan (*Assembly*)
* Menggabungkan komponen *Base* dan *Top Cover* di dalam lingkungan `.SLDASM`.
* Penerapan **Standard Mates** (Concentric, Coincident) untuk memastikan posisi pengunci dan lubang sekrup antar-part sejajar secara mekanis.`
