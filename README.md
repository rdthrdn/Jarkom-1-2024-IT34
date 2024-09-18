![image](https://github.com/user-attachments/assets/cb92eaa5-0884-4817-9aa1-57a0cf1141b3)# Jarkom-1-2024-IT34
Dikerjakan Oleh:
|Nama|NRP |
|--|--|
|Raditya Hardian Santoso|5027231033|
|Rafi Afnaan Fathurahman|5027231040|

## Overview
Pada praktikum modul 1 mata kuliah Komunikasi Data dan Jaringan Komputer kali ini, kita ditugaskan mengerjakan CTF (Capture The Flag) dengan platform yang telah disediakan berjumlah 20 soal. Berikut adalah write up dari soal yang telah kami kerjakan :

### FTP LOGIN (Radit)

![image](https://github.com/user-attachments/assets/199ee009-a10f-4fae-bf8a-98591989c4a5)

Jadi, di soal ini kita perlu mengecek di netcat pertanyaan apa saja yang perlu dijawab untuk mencari flag. Di mana di soal ini pertanyaan yang diperlukan adalah sebagai berikut :

![image](https://github.com/user-attachments/assets/e774e77e-f835-41e0-9121-49a6954f5a5e)

Di sini hal yang ditanyakan adalah username dan password. Dengan menggunakan tools dari wireshark yaitu display filter, jadi saya mencari username dengan mengetik "tcp contains "username"". Lalu, muncul indikasi bahwa username dan password yang salah ditandai dengan tulisan "Login incorrect" sedangkan jika benar tertulis "Login successful". Jadi saya menemukan package yang setelah saya follow tcp menemukan sebagai berikut :

![image](https://github.com/user-attachments/assets/f0bb5209-5ed7-4bed-a1bf-44f345012724)

Di situ tertulis username dan password yang benar. Lalu, kita masukkan ke netcat-nya dan mendapat flagnya.

### CORPORATE BREACH (Radit)

![image](https://github.com/user-attachments/assets/3906d7a6-9b16-4527-acf4-ba53c69e4d31)

Jadi, di soal ini kita perlu mengecek di netcat pertanyaan apa saja yang perlu dijawab untuk mencari flag. Di mana di soal ini pertanyaan yang diperlukan adalah sebagai berikut :

![image](https://github.com/user-attachments/assets/ef82b241-d593-43e7-87d0-aa1974c0a04a)

Di sini hal yang ditanyakan adalah nama attacker, email yang digunakan untuk login beserta passwordnya. Dengan menggunakan tools dari wireshark yaitu export objects, jadi saya bisa melihat file apa saja yang terdapat pada file capture. Di situ terdapat banyak file seperti pada gambar di bawah dan untuk nama dari attackernya terdapat pada file "$2f". Lalu untuk email dan password terdapat pada file package dengan display filter "tcp contains "email" dan scroll ke yang paling bawah karena attacker mengakses paling terakhir. Jadi saya menemukan package yang setelah saya follow tcp menemukan sebagai berikut :

![image](https://github.com/user-attachments/assets/14c491e8-5ff6-492e-a0a7-b6a002ff67ae)
![image](https://github.com/user-attachments/assets/a16de698-d28f-4f36-8ff4-b482e97efc3d)
![image](https://github.com/user-attachments/assets/efaf8fc8-faf5-4e48-8d99-f096466eeb1a)
![image](https://github.com/user-attachments/assets/29b63639-d192-4ccc-9167-fa3a16958598)

Setelah mendapatkan jawaban yang benar. Lalu, kita masukkan ke netcat-nya dan mendapat flagnya.

### ILLEGAL BREAKTHROUGH (Radit)

![image](https://github.com/user-attachments/assets/3906d7a6-9b16-4527-acf4-ba53c69e4d31)

Jadi, di soal ini kita perlu mengecek di netcat pertanyaan apa saja yang perlu dijawab untuk mencari flag. Di mana di soal ini pertanyaan yang diperlukan adalah sebagai berikut :

![image](https://github.com/user-attachments/assets/e49dbc53-cbd5-4236-b048-aeb50309b1f6)

![image](https://github.com/user-attachments/assets/da8260fc-634f-4aee-8523-d3cef596a35d)

Di sini hal yang ditanyakan cukup banyak, di antaranya adalah ip address, port, endpoint, tools apa yang diperlukan, lalu kredensial yang digunakan oleh attacker. Dengan menggunakan tools dari wireshark, saya bisa menemukan hal-hal itu dengan dokumentasi di bawah. Seperti Jadi saya menemukan package yang setelah saya follow tcp menemukan sebagai berikut :

![image](https://github.com/user-attachments/assets/d3dba747-1ec0-4b3e-816b-1ca60d48bd5e)

Setelah mendapatkan jawaban yang benar. Lalu, kita masukkan ke netcat-nya dan mendapat flagnya.

![image](https://github.com/user-attachments/assets/cee75b0d-5465-4e2b-add3-4b99a6176349)


### PACKETS BARRAGE (Radit) :

![image](https://github.com/user-attachments/assets/74dd9265-9ad5-43d3-a4d5-64e4513aec5e)

Jadi, di soal ini kita perlu mengecek di netcat pertanyaan apa saja yang perlu dijawab untuk mencari flag. Di mana di soal ini pertanyaan yang diperlukan adalah sebagai berikut :

![image](https://github.com/user-attachments/assets/f2fd9bdf-136e-45f7-8040-a0fc40f2f9a9)

![image](https://github.com/user-attachments/assets/35b31839-38bc-4808-990a-c8bbe9c1f818)

![image](https://github.com/user-attachments/assets/a4e9c343-5245-46b7-805a-94209825e951)

Di sini hal yang ditanyakan cukup banyak, di antaranya adalah ip address dari attacker, berapa attempt bruteforce yang dilakukan oleh attacker, dan nama file yang didownload oleh attacker. Dengan menggunakan tools dari wireshark, saya bisa menemukan hal-hal itu dengan dokumentasi di bawah. Seperti Jadi saya menemukan package yang setelah saya follow tcp menemukan sebagai berikut :

![image](https://github.com/user-attachments/assets/3da1180e-1a08-41b1-89c2-012737ec72de)

![image](https://github.com/user-attachments/assets/78863a8d-21b1-4710-ae92-7fdadc09a3bf)

![image](https://github.com/user-attachments/assets/68ac8422-2311-43c7-9f96-51ae1f3fb19d)

![image](https://github.com/user-attachments/assets/8a34e30d-21f8-4696-a1ba-3703b7c734ab)

Setelah mendapatkan jawaban yang benar. Lalu, kita masukkan ke netcat-nya dan mendapat flagnya.

![image](https://github.com/user-attachments/assets/808ca143-65de-4611-b87b-d410f4ccbd2a)

### ADVANCE SANITY CHECK (Afnaan) :
### SURPRISE (Afnaan) :
### PEGAWAI NEGERI SEBELAH (Afnaan) :
### EZ (Afnaan) :
### RIZZSET (Afnaan) :
### MALICIOUS CODE (Afnaan) :
### STEGOGRAPHY (Afnaan) :






