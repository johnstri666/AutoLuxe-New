# Title: AUTOLUXE 
# Description
Autoluxe merupakan web yang menampilkan berbagai koleksi mobil dari low-high level dengan berbagai brand mobil di seluruh dunia untuk bisa membantu user dalam menemukan dan membeli mobil impianya. Platform ini dirancang untuk memberikan pengalaman eksklusif bagi pengguna yang mencari informasi detail tentang kendaraan premium, mulai dari spesifikasi teknis hingga galeri foto dan video.

Autoluxe menyediakan solusi yaitu DriveLogic, yang merupakan suatu sistem yang membantu user dalam mengambil keputusan berdasarkan data dan perhitungan untuk menemukan mobil yang sesuai dengan preferensi dan kebutuhan user.

# Tech Used
Frontend: Tailwindcss, HTML5. JS
Backend : Firebase

# Features

1. Sistem autentikasi user dan admin
   - Login and Register
   - Forget Password
   - Sistem berdasarkan peran (user / admin)
  
2. Panel Admin
   - Admin berperan dalam mengelola mobil (edit, add, delete car)
   - Adanya fitur total pengguna website serta total nilai semua mobil yang diinput
   - Field kustom untuk fitur tambahan mobil sehingga akan ditampilkan pada bagiaan ADDITIONAL FEATURES
   - Admin dapat menambahkan foto untuk tiap mobil denga total yang tidak terbatas dan galeri mobil pada bagian bawah setelah menampilkan bagian additional features sebanyak 7 gambar
     
3. Wishlist
   - Menyimpan mobil favorit
   - Hitung total nilai kombinasi kendaraan di wishlist
     
4. Detail Mobil
   - Video showcase
   - Galeri gambar
   - Technical Specification lengkap untuk informasi tiap mobil
   - Audio suara mesin dengan visualizer
   - Filter mobil berdasarkan kategori dan harga

6. User Location
   - Mendeteksi keberadaan user

7. DriveLogic Page
   AutoLuxe juga menghadirkan solusi bagi user yang masih ragu dalam menentukan mobil impiannya.   Dengan memanfaatkan metode TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) pada bagian DriveLogic, AutoLuxe mampu melakukan proses pengambilan keputusan yang tepat. Metode ini menghitung serta menilai berbagai alternatif mobil berdasarkanpreferensi user, sehingga menghasilkan rekomendasi yang paling sesuai dengan kebutuhan dan gaya hidup user.

# Setup Instruction
Clone Repository:

git clone https://github.com/username/autoluxe.git
cd autoluxe

1. Akun Firebase dengan proyek aktif
2. Diperlukan koneksi internet stabil ke Firebase
3. Konfigurasi database
   
import { initializeApp } from "firebase/app";
import { getAnalytics } from "firebase/analytics";

const firebaseConfig = {
  apiKey: "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  authDomain: "xxxxxxxxxxxx",
  projectId: "xxxxxxxxxxxxxxxxxxxxxx",
  storageBucket: "xxxxxxxxxxxxxxxxxxxxxxxxxx",
  messagingSenderId: "6666666666666666666",
  appId: "1:xxxxxxxxxxxxxxxxx",
  measurementId: "G-xxxxxxxxxxxxxxxx"
};

const app = initializeApp(firebaseConfig);
const analytics = getAnalytics(app);

4. Setup Database
- Diperlukan untuk membuat koleksi baru di Firestore database (admins, cars, users).
- Untuk menambahkan admin, tambahkan dokumen dengan ID dokumen yang sama dengan user dan pada koleksi admin, tambahkan role:"admin"
<img width="244" height="85" alt="image" src="https://github.com/user-attachments/assets/c865ce63-25cd-48f8-9938-a0d91c8fedd4" />

# AI Support Explanation
AutoLuxe menggunkana dukungan AI untuk meningkatkan pengalaman pengguna dengan meningkatkan tampilan website serta penambahan fitur yang bertujuan untuk meningkatkan pengalaman user dalam memasuki website AutoLuxe, serta menangani beberap error pada saat membangun proyek ini.


