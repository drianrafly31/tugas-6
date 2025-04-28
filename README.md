# Arsitektur Prosesor: Multiple Processor dan Symmetric Multiprocessor

## Deskripsi
Di dalam arsitektur komputer, terdapat dua model utama yang digunakan untuk mengatur cara prosesor berinteraksi dengan memori dan perangkat keras lainnya, yaitu **Multiple Processor** dan **Symmetric Multiprocessor (SMP)**. Diagram ini membandingkan kedua arsitektur tersebut dengan jelas, menampilkan komponen-komponen utama dan bagaimana mereka saling berinteraksi.

### 1. **Multiple Processor**  
Pada arsitektur ini, terdapat beberapa prosesor yang terhubung dengan satu unit memori utama melalui sebuah bus. Setiap prosesor memiliki memori privat (seperti cache L1), dan menggunakan bus arbiter untuk mengatur akses ke memori bersama. Arsitektur ini umumnya lebih sederhana dan digunakan untuk aplikasi yang tidak memerlukan tingkat kecepatan komunikasi yang sangat tinggi antar prosesor.

**Komponen:**
- **Prosesor**: Unit pemrosesan yang menjalankan instruksi.
- **Cache L1**: Cache privat untuk setiap prosesor, berfungsi untuk mempercepat akses data.
- **Bus Arbiter**: Menangani akses ke memori utama untuk beberapa prosesor.
- **Memori Utama**: Tempat penyimpanan data yang digunakan bersama oleh semua prosesor.

### 2. **Symmetric Multiprocessor (SMP)**  
Arsitektur SMP lebih kompleks, di mana beberapa prosesor berbagi akses ke memori bersama. Setiap prosesor memiliki cache privat L1, tetapi juga terhubung ke cache L2 yang digunakan bersama oleh semua prosesor. Dalam sistem SMP, prosesor dapat saling berkomunikasi lebih cepat dan lebih efisien, membuatnya lebih cocok untuk aplikasi yang membutuhkan komputasi paralel yang besar.

**Komponen:**
- **Prosesor**: Beberapa unit pemrosesan yang dapat beroperasi secara independen tetapi berbagi akses ke memori.
- **Cache L1**: Cache privat untuk setiap prosesor.
- **Cache L2**: Cache bersama yang digunakan oleh semua prosesor untuk meningkatkan efisiensi akses data.
- **Memori Utama**: Memori yang digunakan bersama oleh semua prosesor, memungkinkan akses lebih cepat untuk data yang sering digunakan.

## Tujuan Diagram
Diagram ini dirancang untuk memberikan gambaran yang lebih jelas mengenai perbedaan antara arsitektur **Multiple Processor** dan **Symmetric Multiprocessor (SMP)**, dengan menampilkan elemen-elemen penting yang membentuk kedua arsitektur tersebut.

- **Multiple Processor** lebih sederhana, dengan beberapa prosesor yang terhubung ke memori utama.
- **Symmetric Multiprocessor** memungkinkan komunikasi lebih efisien antar prosesor berkat adanya cache bersama L2.

## Cara Penggunaan
Diagram ini dapat digunakan untuk memahami struktur dasar dari kedua arsitektur dan bagaimana mereka mengelola memori dan prosesor dalam sebuah sistem komputer. Anda dapat memodifikasi diagram ini menggunakan alat seperti **draw.io** untuk menyesuaikan dengan kebutuhan desain lebih lanjut atau menambahkan komponen lainnya.

## Diagram

![labeled-multiprocessor-diagram](https://github.com/user-attachments/assets/69a2909b-ec32-4102-9bef-5eda2124fd0d)



