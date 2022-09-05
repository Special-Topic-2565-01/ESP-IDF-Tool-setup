# ESP-IDF Tool 
 
IDF ย่อมาจาก IoT Development Framework เป็น framework สำหรับพัฒนา IoT ที่ดูแลโดย  Espressif ที่เป็นผู้ผลิตชิบ ESP32 ซึ่งปัจจุบันมีออกมาหลายรุ่น ได้แก่ ESP32, ESP32-S, ESP32-C และ ESP32-H
ศึกษารายละเอียดเพิ่มเติมได้จาก https://www.espressif.com/en/products/sdks/esp-idf


## การติดตั้งเครื่องมือพัฒนา IoT  บน ESP32



1. Download ไฟล์ติดตั้งจาก https://dl.espressif.com/dl/esp-idf/


<p align="center">
<img  src="Pictures/Image-01.png" alt="Image 001" style="width:400px;" >
</p>


เลือก Espressif-IDE x.x.x with ESP-IDF vx.x.x เพื่อติดตั้งทั้ง IDE  และ ESP-IDF

- IDE ที่ติดตั้งจะเป็น IDE ที่พัฒนามาจากโปรแกรม editor ที่ชื่อ Eclipse มีความสามารถในการทำงานกับโปรเจคในภาษาต่างๆ รวมทั้งทำงานร่วมกับ git ซึ่ง Espressif ได้รวมเอาความสามารถเหล่านั้นไว้ใน Espressif-IDE เรียบร้อยแล้ว (และเราก็สามารถติดตั้ง plugins ของ Eclipse เพิ่มเติมได้ตามต้องการ)
- ESP-IDF  ย่อมาจาก ESP IoT Development Framework เป็น framework ที่รวมเอาชุดพัฒนาในภาษา C/C++ ทั้ง compiler, linker, locator และ script ต่างๆ เพื่อการดึง Library ต่างๆ มาร่วมทำงานบน IDE


## ขั้นตอนการติดตั้ง

ดำเนินการติดตั้งตามขั้นตอนต่อไปนี้  [ESP-IDF setup](esp-idf-setup.md)