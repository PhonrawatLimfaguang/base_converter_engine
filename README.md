# 🧮 base_converter_engine

เครื่องมือคำนวณทางคณิตศาสตร์และระบบแปลงเลขฐาน (Base-N Converter) พัฒนาด้วย Python โดยเน้นความถูกต้องของข้อมูล (Data Integrity) และการจัดการข้อผิดพลาด (Exception Handling)

## 🚀 Key Capabilities

### 1. Robust Calculator Engine
* **Continuous Operation:** รองรับการคำนวณต่อเนื่อง (Chained Calculations) โดยนำผลลัพธ์เดิมมาใช้ต่อได้ทันที
* **Zero-Error Tolerance:** มีระบบดักจับการหารด้วยศูนย์ (Division by Zero Protection) เพื่อป้องกัน Runtime Crash
* **Precision Handling:** ควบคุมทศนิยม 3 ตำแหน่งอัตโนมัติ เพื่อความสวยงามและแม่นยำในการแสดงผล

### 2. Number System Converter (Hex/Bin/Dec)
* **Algorithm:** ใช้อัลกอริทึม **Intermediate Decimal Conversion** เพื่อความแม่นยำสูงสุดในการแปลงข้ามฐาน
* **Supports:**
    * Binary (Base 2) ↔ Decimal (Base 10)
    * Hexadecimal (Base 16) ↔ Binary (Base 2)
    * Decimal (Base 10) ↔ Hexadecimal (Base 16)

### 3. User Input Validation
* ป้องกันการใส่ข้อมูลผิดประเภท (เช่น ใส่ตัวอักษรในช่องตัวเลข) ด้วย `try...except` block
* ระบบแจ้งเตือน (Interactive Feedback) เมื่อผู้ใช้ป้อน Operator ผิด

## 🛠️ Logic & Algorithms
โค้ดถูกออกแบบโดยใช้หลักการ **Modular Programming** แยกฟังก์ชันการทำงานชัดเจน:
* `get_number_input(base)`: ฟังก์ชันตรวจสอบ Data Type ตามฐานที่เลือก
* `calculate_result(...)`: Core Logic สำหรับประมวลผลทางคณิตศาสตร์
* `convert_base(...)`: Algorithm สำหรับการแปลงค่าระหว่างฐานข้อมูล

## 📦 How to Use
1.  Open `base_converter_engine.ipynb` in Jupyter Notebook or Google Colab.
2.  Run the main cell to start the interactive CLI.
3.  Follow the on-screen prompts to select 'Calculator' or 'Converter' mode.

---
**Developed as part of Data Engineering coursework (DE113 OOP)**
*Demonstrating fundamental Python logic and control flow mastery.*
