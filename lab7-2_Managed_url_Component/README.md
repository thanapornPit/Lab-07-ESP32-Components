# Lab 7-2: Managed Component from GitHub URL Demo


## ผลลัพธ์ที่คาดหวัง
- แสดงข้อความการเริ่มต้น sensor จาก GitHub component
- แสดงข้อมูล temperature และ humidity ทุก 4 วินาที
- แสดงสถานะการทำงานของ sensor
- แสดงแหล่งที่มาของ component (GitHub Repository)

## ความแตกต่างจาก Lab 7-1
- Lab 7-1: ใช้ local component (ในเครื่อง)
- Lab 7-2: ใช้ managed component จาก GitHub URL

## การใช้งาน
1. เข้าไปในโฟลเดอร์ lab7-2_Managed_url_Component
2. รันคำสั่ง `idf.py build` (จะดาวน์โหลด component จาก GitHub อัตโนมัติ)
3. ทดสอบด้วย QEMU
<img width="878" height="462" alt="image" src="https://github.com/user-attachments/assets/d48f76a8-8695-4e2e-8901-be8c578254e8" />







## โจทย์ท้าทาย

สร้าง component ชื่อ Display โดย นำไฟล์ display.c และ display.h จากใบงานที่ 6 มาใช้

นำโค้ดจาก main.c ในใบงานที่ 6 มาใช้ แล้ว build พร้อมทดสอบ ให้ผลลักษณะเดียวกับ component แบบ local หรือไม่
