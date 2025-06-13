# Family Map - ระบบจัดการบ้านและผังเครือญาติ V1.0.0

ระบบนี้พัฒนาเพื่อจัดเก็บข้อมูลสมาชิกภายในบ้าน และแสดงผังเครือญาติอย่างเป็นระบบ โดยใช้ PHP และฐานข้อมูล MySQL

## 📌 คุณสมบัติ (Features)

- บันทึกข้อมูลบ้านและสมาชิกในครอบครัว
- แสดงผังเครือญาติหรือความสัมพันธ์ระหว่างบุคคล
- เรียกดูและจัดการข้อมูลผ่าน API (`api.php`)
- การเชื่อมต่อฐานข้อมูลผ่าน `config.php`

## ⚙️ ความต้องการระบบ (Requirements)

- PHP >= 7.4
- MySQL หรือ MariaDB
- Apache/Nginx Web Server (เช่น XAMPP, MAMP, Laragon)

## 🚀 วิธีการติดตั้ง (Installation)

1. **Clone โปรเจกต์จาก GitHub**
   ```bash
   git clone https://github.com/maewongh/family-map.git
   cd family-map
สร้างฐานข้อมูล

เปิด phpMyAdmin หรือใช้เครื่องมือจัดการฐานข้อมูลอื่น

สร้างฐานข้อมูลใหม่ชื่อ house_management

นำเข้าไฟล์ house_management.sql ที่อยู่ในโปรเจกต์:

bash
Copy
Edit
mysql -u root -p house_management < house_management.sql
ตั้งค่าการเชื่อมต่อฐานข้อมูล

เปิดไฟล์ config.php แล้วแก้ไขค่าต่อไปนี้ให้ตรงกับระบบของคุณ:

php
Copy
Edit
$host = 'localhost';
$dbname = 'house_management';
$username = 'root';
$password = '';
เรียกใช้งานระบบ

เปิดเบราว์เซอร์แล้วเข้า URL:

perl
Copy
Edit
http://localhost/family-map/
🗂️ โครงสร้างไฟล์โปรเจกต์
📄 License
Distributed under the MIT License.

👤 ผู้พัฒนา
Narachai60

GitHub: maewongh
Copy
Edit
   ```bash
   ├── api.php                  # จัดการคำขอ API
   ├── config.php               # ตั้งค่าฐานข้อมูล
   ├── house_management.sql     # ไฟล์ฐานข้อมูล
   ├── index.php                # หน้าเริ่มต้นของระบบ
   └── README.md

