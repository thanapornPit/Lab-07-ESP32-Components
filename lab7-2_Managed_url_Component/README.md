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
```bash
 I (8003) MAIN: === Loop 0 ===
 I (8003) DISPLAY: 🧹 Screen cleared from file: ./managed_components/lab7_components/Display/display.c, line: 28
 I (8003) DISPLAY: ✨ Display ready for new content
 I (8003) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
 I (8003) SENSOR: 🌡️  Temperature: 30.7°C
 I (8013) SENSOR: 💧 Humidity: 84.2%
 I (8013) DISPLAY: 📊 Data display from file: ./managed_components/lab7_components/Display/display.c, line: 21
 I (8023) DISPLAY: 📈 Value 1: 26.50
 I (8023) DISPLAY: 📉 Value 2: 61.00
 I (10023) MAIN: === Loop 1 ===
 I (10023) DISPLAY: 🧹 Screen cleared from file: ./managed_components/lab7_components/Display/display.c, line: 28
 I (10023) DISPLAY: ✨ Display ready for new content
 I (10023) SENSOR: 📊 Reading sensor data from file: ./managed_components/lab7_components/Sensors/sensor.c, line: 18
 I (10023) SENSOR: 🌡️  Temperature: 30.2°C
 I (10023) SENSOR: 💧 Humidity: 79.0%
 I (10023) DISPLAY: 📊 Data display from file: ./managed_components/lab7_components/Display/display.c, line: 21
 I (10023) DISPLAY: 📈 Value 1: 27.50
 I (10023) DISPLAY: 📉 Value 2: 62.00

```
