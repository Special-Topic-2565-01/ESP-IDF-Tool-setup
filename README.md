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

1. เมื่อ download ไฟล์มาแล้ว ให้เรียกขึ้นมาทำงาน

2. จะปรากฏหน้าจอ License Agreement ให้อ่านทำความเข้าใจ ถ้ายอมรับให้เลือก I accept the agreement. แล้วคลิกปุ่ม Next เพื่อดำเนินการขั้นถัดไป

<p align="center">
<img  src="Pictures/Setup-01.png" alt="Setup 01" style="width:400px;" >
</p>

3. ตัวติดตั้งจะตรวจสอบความพร้อมของระบบและสภาพแวดล้อมของเครื่องคอมพิวเตอร์ที่จะติดตั้ง (Pre-installation system check) และรายงานออกมา ถ้ามีบางอย่างที่ไม่เข้ากัน (สังเกตุจากปุ่ม Apply Fixed จะ Active) ให้กดปุ่ม Apply Fixed เพื่อให้ตัวติดตั้งทำการปรับปรุงระบบให้เหมาะกับการติดตั้ง ซึ่งอาจจะต้องให้ผู้ใช้อนุญาตการกระทำนั้น ให้ตอบตกลงในกรณีที่มีหน้าจอขออนุญาตแสดงขึ้นมา จากนั้นกดปุ่ม `Next` เพื่อดำเนินการขั้นถัดไป

<p align="center">
<img  src="Pictures/Setup-02.png" alt="Setup 02" style="width:400px;" >
</p>

4. ตัวติดตั้งจะถามตำแหน่งที่ต้องการติดตั้ง ในกรณีที่เป็นคอมพิวเตอร์ส่วนบุคคล อาจจะติดตั้งในตำแหน่งที่ตัวติดตั้งกำหนดไว้เป็นค่าเริ่มต้น `(C:\Epressif)` แต่ถ้าใช้เครื่องคอมพิวเตอร์ส่วนรวมหรือมีเนื้อที่ในไดรว์ C ไม่เพียงพอ อาจจะต้องเลือกตำแหน่งสำหรับติดตั้งที่เหมาะสม จากนั้นกดปุ่ม `Next` เพื่อดำเนินการขั้นถัดไป 

<p align="center">
<img  src="Pictures/Setup-03.png" alt="Setup 03" style="width:400px;" >
</p>

5. ตัวติดตั้งจะถามรูปแบบการติดตั้งที่ต้องการ หากมีเนื้อที่เพียงพอ แนะนำให้เลือกแบบ Full installation แต่ถ้าต้องการประหยัดพื้นที่ ก็อาจจะเลือก Minimal installation หรืออาจจะกำหนดองค์ประกอบที่ต้องการเอง (Customize installation) เสร็จแล้วกดปุ่ม `Next` เพื่อดำเนินการขั้นถัดไป

<p align="center">
<img  src="Pictures/Setup-04.png" alt="Setup 04" style="width:400px;" >
</p>

6. ตัวติดตั้งจะรายงานรายการที่จะทำการติดตั้ง โดยแจ้งว่า Ready to Install ในขั้นนี้ ถ้าพร้อมจะติดตั้ง ไม่มีสิ่งใดต้องการแก้ไข ก็ให้กดปุ่ม `Next` เพื่อติดตั้ง (ซึ่งหลังจากนี้จะเป็นการดำเนินการโดยตัวติดตั้งจนเสร็จ ไม่สามารถย้อนกลับได้)

<p align="center">
<img  src="Pictures/Setup-05.png" alt="Setup 05" style="width:400px;" >
</p>

7. ตัวติดตั้งจะเตรียมการติดตั้ง

<p align="center">
<img  src="Pictures/Setup-06.png" alt="Setup 06" style="width:400px;" >
</p>

8.  ตัวติดตั้งดำเนินการติดตั้ง อาจจะมีกล่องโต้ตอบเพื่อขออนุญาตแก้ไขระบบ ถ้าพิจารณาแล้วไม่เกิดปัญหา ให้อนุญาตให้ตัวติดตั้งทำการปรับปรุงระบบ

<p align="center">
<img  src="Pictures/Setup-07.png" alt="Setup 07" style="width:400px;" >
</p>

9. เมื่อติดตั้งเรียบร้อย ตัวติดตั้งจะทำการกำหนด python environment ที่จะช่วยในการ build firmware binary จาก project ที่เราสร้าง

<p align="center">
<img  src="Pictures/Setup-08.png" alt="Setup 08" style="width:400px;" >
</p>

10. การติดตั้งเรียบร้อย ตัวติดตั้งให้โอกาสในการตั้งค่า Environment ของระบบเพื่อให้สามารถเรียกใช้ซอฟต์แวร์ได้จาก command line ถ้าต้องการให้ติ๊กตัวเลือก `Run ESP-IDF PowerShell Environment` และ `Run ESP-IDF Command Prompt Environment` กดปุ่ม `Next` เพื่อดำเนินการขั้นถัดไป
     

<p align="center">
<img  src="Pictures/Setup-09.png" alt="Setup 09" style="width:400px;" >
</p>

11.  จะปรากฏหน้าจอ `ESP-IDF 4.4 CMD` เมื่อรันจนปรากฏข้อความ `C:\......\esp-idf-v4.4.2` แล้ว สามารถปิดหน้าต่างนี้ได้ 

<p align="center">
<img  src="Pictures/Setup-10.png" alt="Setup 10" style="width:400px;" >
</p>


12.  จะปรากฏหน้าจอ `ESP-IDF 4.4 PowerShell` เมื่อรันจนปรากฏข้อความ `PS C:\......\esp-idf-v4.4.2` แล้ว สามารถปิดหน้าต่างนี้ได้ 

<p align="center">
<img  src="Pictures/Setup-11.png" alt="Setup 11" style="width:400px;" >
</p>

13. ถ้าการติดตั้งทุกอย่างเป็นไปด้วยความเรียบร้อย จะมีซอฟต์แวร์ของ Espressif ติดตั้งบนเครื่อง สามารถเรียกใช้งานได้จากไอคอนด้านล่างนี้

<p align="center">
<img  src="Pictures/Setup-12.png" alt="Setup 12" style="width:150px;" >
</p>

