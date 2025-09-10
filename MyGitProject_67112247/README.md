# รายงานการบ้าน Git Branch / Merge

## ข้อมูลผู้จัดทำ
- ชื่อ: วิรดา สุทธสิทธิ์  
- รหัสนักศึกษา: 67112247

## วัตถุประสงค์
เพื่อฝึกการใช้งาน Git ในการสร้าง branch และ merge branch เข้ากับ main พร้อมทั้งบันทึกขั้นตอนการทำงานและจัดทำรายงานสรุป

## ขั้นตอนการดำเนินงาน
1. สร้าง Git repository ใหม่ และตั้ง branch หลักชื่อ `main`  
2. ทำการ commit แรก โดยเพิ่มโฟลเดอร์ `test001` และไฟล์ `README.md`  
3. สร้าง branch ชื่อ `FromTest2` แล้วเพิ่มโฟลเดอร์ `test002` และไฟล์ `myfunc2.py`  
   - ภายใน `myfunc2.py` มีฟังก์ชัน `add(a, b)` สำหรับบวกเลข 2 ตัว  
4. กลับไปที่ branch `main` แล้วทำการ merge branch `FromTest2` เข้ามา  
5. แก้ไขไฟล์ `README.md` เพื่อสรุปขั้นตอนและบันทึกหลักฐานการดำเนินงาน 

## หลักฐานการดำเนินงาน

### 1. รายชื่อ branch
    git branch -a

### 2. กราฟ commit
    git log --oneline --graph --decorate --all

### 3. โครงสร้างไฟล์หลัง merge
    tree /F

### 4.ผลลัพท์จากการทำ เพิ่ม ไฟล์ myfunc2.py ตามโจรท์ ที่มีฟังก์ชันการดำเนินการ ลบ เลข 2 ชุด
    โค้ด ไฟล์ myfunc2.py
    def add(a, b):
    return a - b

    if __name__ == "__main__":
    print(add(3, 2))

### 4. Screenshot การทำงาน
![Branch](![alt text](image.png))  
![Log](![alt text](image-1.png))  
![Tree](![alt text](image-2.png))  
![README](![alt text](image-3.png))
![myfunc2.py](![alt text](image-4.png))


