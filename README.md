<img width="553" height="274" alt="image" src="https://github.com/user-attachments/assets/abdb29fc-ce7c-4b19-8c61-1dd91b763a43" /># Title: AUTOLUXE 
# Description

<img width="1298" height="628" alt="image" src="https://github.com/user-attachments/assets/aab89b74-0244-4693-8701-2327cc138f28" />

Autoluxe merupakan web yang menampilkan berbagai koleksi mobil dari low-high level dengan berbagai brand mobil di seluruh dunia untuk bisa membantu user dalam menemukan dan membeli mobil impianya. Platform ini dirancang untuk memberikan pengalaman eksklusif bagi pengguna yang mencari informasi detail tentang kendaraan premium, mulai dari spesifikasi teknis hingga galeri foto dan video.

Autoluxe menyediakan solusi yaitu DriveLogic, yang merupakan suatu sistem yang membantu user dalam mengambil keputusan berdasarkan data dan perhitungan untuk menemukan mobil yang sesuai dengan preferensi dan kebutuhan user.

# Tech Used
Frontend: Tailwindcss, HTML5. JS
Backend : Firebase

# Features
1. Sistem autentikasi user dan admin
   - Login and Register
     <img width="523" height="233" alt="image" src="https://github.com/user-attachments/assets/2322a94d-c8c9-4092-ae8e-217eb4ea7a53" />

   - Forget Password
     <img width="553" height="274" alt="image" src="https://github.com/user-attachments/assets/d5cf5c5b-d47b-413e-ba2b-506bca6fa9ee" />

   - Sistem berdasarkan peran (user / admin)
  
2. Panel Admin
   - Admin berperan dalam mengelola mobil (edit, add, delete car)
     <img width="976" height="527" alt="image" src="https://github.com/user-attachments/assets/4ff5e552-5b65-4443-9156-bb325510a843" />

   - Adanya fitur total pengguna website serta total nilai semua mobil yang diinput
        <img width="1176" height="568" alt="image" src="https://github.com/user-attachments/assets/eaa52f56-b075-492b-b577-98b83e901f91" />
   - Field kustom untuk fitur tambahan mobil sehingga akan ditampilkan pada bagiaan ADDITIONAL FEATURES
   <img width="1080" height="538" alt="image" src="https://github.com/user-attachments/assets/c16edcb8-8cde-4119-aca7-183f62163711" />

   - Admin dapat menambahkan foto untuk tiap mobil dengan total yang tidak terbatas dan galeri mobil pada bagian bawah setelah menampilkan bagian additional features sebanyak 7 gambar
<img width="1181" height="569" alt="image" src="https://github.com/user-attachments/assets/0ecdbe53-2a42-4419-a2fa-11ef11cc40c9" />

3. Wishlist
   - Menyimpan mobil favorit serta total nilai kombinasi kendaraan di wishlist
   <img width="1211" height="558" alt="image" src="https://github.com/user-attachments/assets/5bef7ecb-48b6-4eba-b9c7-998b09f3dd87" />

4. Detail Mobil
   - Video showcase
   - Galeri gambar
   - Technical Specification lengkap untuk informasi tiap mobil
   - Audio suara mesin dengan visualizer
   - Filter mobil berdasarkan kategori dan harga

<img width="834" height="555" alt="image" src="https://github.com/user-attachments/assets/79a863b5-0e24-4a6e-9cd5-57d8cc0285d0" />

<img width="838" height="579" alt="image" src="https://github.com/user-attachments/assets/8eb3407e-c406-4583-acee-66779d911b24" />

<img width="931" height="593" alt="image" src="https://github.com/user-attachments/assets/a28916e6-d5c8-4782-9c02-05d659430d45" />

<img width="1017" height="571" alt="image" src="https://github.com/user-attachments/assets/2274112d-9829-4c0d-b6d8-d54f43874ec2" />


5. User Location
   - Mendeteksi keberadaan user

6. DriveLogic Page
<img width="1200" height="629" alt="image" src="https://github.com/user-attachments/assets/65ceeaaa-56f7-46d0-bcf4-5161c3f02879" />

<img width="1242" height="624" alt="image" src="https://github.com/user-attachments/assets/d6823ee7-9a41-43f4-b79b-91816c6e82f0" /> 

AutoLuxe juga menghadirkan solusi bagi user yang masih ragu dalam menentukan mobil impiannya.   Dengan memanfaatkan metode TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) pada bagian DriveLogic, AutoLuxe mampu melakukan proses pengambilan keputusan yang tepat. Metode ini menghitung serta menilai berbagai alternatif mobil berdasarkanpreferensi user, sehingga menghasilkan rekomendasi yang paling sesuai dengan kebutuhan dan gaya hidup user.

# Setup Instruction
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


