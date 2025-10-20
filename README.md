# XLMRat-Network-Compromise-and-PCAP-Investigation
Laporan ini merupakan hasil investigasi tim SOC terhadap file packet capture (PCAP) yang diperoleh dari perangkat network analyzer untuk mengidentifikasi aktivitas awal infeksi malware dan pola komunikasi yang mengindikasikan adanya tindakan berbahaya. Dari hasil analisa ditemukan koneksi mencurigakan menuju IP publik 45.126.209.4, di mana file xlm.txt yang diunduh melalui protokol HTTP berisi obfuscated payload yang menjalankan perintah PowerShell guna mengunduh file mdm.jpg, yang teridentifikasi sebagai varian AsyncRAT. Malware tersebut diketahui memanfaatkan legitimate tools seperti RegSvcs.exe untuk menjalankan prosesnya di memori serta membuat scheduled task guna mempertahankan persistensi. Berdasarkan temuan tersebut, insiden ini dikategorikan sebagai infeksi Remote Access Trojan (RAT) yang menggunakan teknik defense evasion dan persistence untuk menghindari deteksi serta mempertahankan akses ke sistem korban. 

<img width="818" height="371" alt="image" src="https://github.com/user-attachments/assets/e64e608a-b651-4203-ba11-5dcb6a2c2739" />

<img width="940" height="523" alt="image" src="https://github.com/user-attachments/assets/9135c3c9-b04e-4936-bc85-243e62db40cb" />




