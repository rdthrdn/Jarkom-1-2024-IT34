# Jarkom-1-IT34-2024
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

![image](https://github.com/user-attachments/assets/af6faf94-83a2-486a-bcd5-01ba47b60977)

Setelah melakukan netcat, muncul pertanyaan pertanyaan seperti berikut:
![image](https://github.com/user-attachments/assets/17827851-545c-4c9b-a1a5-7f586bdb8c48)

Untuk pertanyaan pertama, bisa didapatkan dengan follow stream TCP dan menaikkan stream sampai benar
![image](https://github.com/user-attachments/assets/042e05dd-428e-4510-add4-6ee3a2c56c38)

Untuk pertanyaan kedua, dilanjutkan follow stream sampai dapat nama file dan extension
![image](https://github.com/user-attachments/assets/e1e8ffc4-3f8f-42ca-a3da-659c5999c8c0)

Untuk pertanyaan ketiga, periksa bagian MIME dan ikuti arahannya. Lalu decrypt menggunakan base64
![image](https://github.com/user-attachments/assets/b117cc06-bddf-423a-8ab4-3efa27d1fff9)
![image](https://github.com/user-attachments/assets/fd41a074-9908-4f3b-8477-9c35f4acb92a)
![image](https://github.com/user-attachments/assets/63ad1a73-2679-42e8-b49c-3022197c3dfd)

### SURPRISE (Afnaan) :

![image](https://github.com/user-attachments/assets/3851e8d9-c7d1-4aa3-a7dd-436ccab275f8)

Berikut pertanyaannya:
![image](https://github.com/user-attachments/assets/f10f4293-7b83-482e-920c-9d3fe2091750)

Untuk 2 soal pertama dapat ditemukan jawabannya dengan follow stream TCP
![image](https://github.com/user-attachments/assets/44e0511d-4728-4a8a-a195-5ad71905a759)
![image](https://github.com/user-attachments/assets/8b8368e9-4d0a-47f5-b3be-4e845169731b)

Untuk soal ketiga, file dapat diambil dengan 2 cara. Export object as FTP-Data atau follow stream dan mengambil manual
![image](https://github.com/user-attachments/assets/d2a300d4-8f8b-4219-9795-c1a06ae04f6c)

Setelah dijalankan, akan didapatkan output sebagai jawaban pertanyaan ketiga
![image](https://github.com/user-attachments/assets/c2d4ad22-4402-4d26-9aae-56061782d5a3)

### PEGAWAI NEGERI SEBELAH (Afnaan) :

![image](https://github.com/user-attachments/assets/137b4b0e-f465-477c-8e5d-5a1f5ac739b9)

Berikut pertanyaannya:
![image](https://github.com/user-attachments/assets/dded1310-5c4d-4324-b482-13ae91c31b01)

Untuk semua pertanyaan, jawabannya bisa ditemukan di csv ini dan dapat dengan mudah dicari dengan fungsi find
![image](https://github.com/user-attachments/assets/d59757fb-42f4-4f35-82e8-31ff9ce172ad)

### EZ (Afnaan) :

![image](https://github.com/user-attachments/assets/54bdd62d-4402-4508-82c2-526cf96b1ec2)

Berikut pertanyaannya:
![image](https://github.com/user-attachments/assets/38f0e6e7-ef81-407d-95e2-9b1ecaeeb2f6)

Untuk pertanyaan pertama bisa didapatkan dengan follow TCP stream
![image](https://github.com/user-attachments/assets/589f93d6-6331-426a-8340-55b18745310f)

Untuk pertanyaan kedua bisa didapatkan dengan melihat ke wireshark
![image](https://github.com/user-attachments/assets/1befadd6-4f71-400e-a320-9e2a9d0c9ce1)

### RIZZSET (Afnaan) :

![image](https://github.com/user-attachments/assets/c38d79d5-dfc7-4f82-8293-9b42a6601468)

Berikut pertanyaannya:
![image](https://github.com/user-attachments/assets/f94f4877-53be-4208-b87d-f500756151d7)

Untuk pertanyaan pertama bisa didapatkan dari follow UDP stream
![image](https://github.com/user-attachments/assets/128f7e79-2b2a-4db9-8898-fa4e379aec00)

Untuk pertanyaan kedua, bisa lanjut follow UDP stream dan membaca angka dari belakang
![image](https://github.com/user-attachments/assets/d39e659f-c2c9-449d-98d9-202cd837a2f4)

Untuk pertanyaan terakhir, harus menggunakan tool external yaitu JARM
https://github.com/salesforce/jarm
![image](https://github.com/user-attachments/assets/fbd61eb7-06ad-4073-ab88-fc282eb8196d)

### MALICIOUS CODE (Afnaan) :

![image](https://github.com/user-attachments/assets/01961d1f-2c26-495e-8d4e-063a0eb21bec)

Berikut pertanyaannya:
![image](https://github.com/user-attachments/assets/13e1b9a2-37cf-4f27-a40b-59a869b3b00a)

Untuk pertanyaan pertama, bisa menggunakan filter `frame contains "GET"` dan melihat berapa packet yang muncul
![image](https://github.com/user-attachments/assets/2f97f3ec-6017-4978-97f0-4d5c978f08c2)

Untuk pertanyaan kedua, bisa melihat packet terakhir dari filter di soal sebelumnya
![image](https://github.com/user-attachments/assets/47c0f2fa-f099-43f2-81ae-c0ea5cd7a2e3)

Untuk pertanyaan ketiga, bisa menggunakan filter `frame contains "password="` dan memilih yang tidak diprompt untuk memasukkan password lagi
![image](https://github.com/user-attachments/assets/f999f240-3dcf-4efc-8d29-b52ce37496b5)

Untuk pertanyaan keempat, follow terus sampai mendapatkan pertanyaan lalu di translate dan dijawab (jawabannya sudah sangat jelas merah)
![image](https://github.com/user-attachments/assets/bf737d5a-839d-4518-9979-9e2afe7753fa)
![image](https://github.com/user-attachments/assets/7484a65d-2d8d-4ed8-87f8-91ff7ea8bc6b)

### STEGOGRAPHY (Afnaan) :

![image](https://github.com/user-attachments/assets/ef8b5252-7fd4-4ccc-a7cb-6a069fd8a6e6)

Berikut adalah pertanyaannya:
![image](https://github.com/user-attachments/assets/ceec90d3-e8f2-4fd7-86d9-ef9f56795ff8)

Untuk pertanyaan pertama, export object semua file yang tersedia dan hitung jumlah file .png
![image](https://github.com/user-attachments/assets/8f65e9e5-56ed-4b5a-aa1b-95b00186ed67)

Untuk pertanyaan kedua dan ketiga, perbaiki code python dan gunakan untuk memeriksa masing masing png
```python
import sys
from PIL import Image

def decode_image_reversed(image_path):
    img = Image.open(image_path)
    img = img.convert("RGB")
    pixels = img.load()

    binary_message = ""
    for i in range(img.width):
        for j in range(img.height):
            r, g, b = pixels[i, j]
            
            r_bin = format(r, '08b')
            binary_message += r_bin[-1]

    message = ""
    for i in range(0, len(binary_message), 8):
        byte = binary_message[i:i + 8]
        char = chr(int(byte, 2))
        
        if message.endswith("EOF"):
            break
        message += char

    message = message.replace("EOF", "")

    reversed_message = message[::-1]
    return reversed_message

if __name__ == "__main__":
    if len(sys.argv) < 2:
        print("Usage: python script.py <image_path>")
    else:
        image_path = sys.argv[1]
        decoded_message_reversed = decode_image_reversed(image_path)
        print(f"Pesan terbalik yang diambil: {decoded_message_reversed}")
```
![image](https://github.com/user-attachments/assets/a6920063-1716-4c61-9e53-73947c410607)

---
## REVISI
---

### GAJAH TERBANG (ATTACKER RECON) :
![image](https://github.com/user-attachments/assets/d3923366-fd32-4a38-bf0d-dc2d54340ba5)
![image](https://github.com/user-attachments/assets/6594da07-08ef-4c53-81fb-fcbb692d0cfc)

### BABY HENGKER :
![image](https://github.com/user-attachments/assets/7552e5ce-3b0d-4bb0-93ea-4ba10e00e504)
![image](https://github.com/user-attachments/assets/19ac7e0f-c297-456c-bae1-df3f77c788d4)

### ADULT HENGKER :
![image](https://github.com/user-attachments/assets/872c118b-bace-4f59-acb9-2a157c5314d8)
![image](https://github.com/user-attachments/assets/2ed319cc-6b9e-4751-9221-32db3520c619)
![image](https://github.com/user-attachments/assets/174691c8-d266-4f6d-82ae-f5599eeb6b89)
![image](https://github.com/user-attachments/assets/060b2239-636c-484a-b2c1-9caeb45acfa2)








