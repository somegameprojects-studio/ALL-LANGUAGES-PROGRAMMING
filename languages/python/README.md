# คู่มือ Python ภาษาไทย

Python เป็นภาษาโปรแกรมระดับสูงที่เน้นอ่านง่าย ใช้ทำเว็บ งานอัตโนมัติ วิเคราะห์ข้อมูล วิทยาศาสตร์ และ AI ได้

## 1. เตรียมเครื่องมือ

ติดตั้ง Python จาก [python.org](https://www.python.org/downloads/) แล้วตรวจรุ่นด้วย `python --version` (บางระบบใช้ `python3 --version`) สร้างไฟล์ชื่อ `main.py` แล้วสั่ง `python main.py`

## 2. แสดงผลและตัวแปร

```python
name = "Mina"
age = 13
print("สวัสดี", name)
print("ปีหน้าอายุ", age + 1)
```

- `name` เก็บข้อความ
- `age` เก็บจำนวนเต็ม
- `print()` แสดงข้อมูล

## 3. รับข้อมูลและเงื่อนไข

```python
score = int(input("คะแนน: "))
if score >= 50:
    print("ผ่าน")
else:
    print("ลองใหม่")
```

`input()` ได้ข้อความ จึงแปลงเป็นจำนวนเต็มด้วย `int()` ก่อนเปรียบเทียบ

## 4. ลูปและฟังก์ชัน

```python
for number in range(1, 4):
    print(number)

def greet(person):
    return "สวัสดี " + person

print(greet("Mina"))
```

## 5. ข้อผิดพลาดที่พบบ่อย

- `SyntaxError`: เขียนรูปแบบคำสั่งไม่ถูก
- `NameError`: เรียกชื่อตัวแปรที่ไม่มี
- `TypeError`: ใช้ข้อมูลต่างชนิดกันไม่ถูกวิธี
- Python ใช้การเยื้องบรรทัดเพื่อแบ่งบล็อกคำสั่ง

## 6. แบบฝึกหัด

1. รับชื่อผู้ใช้แล้วทักทาย
2. รับตัวเลขแล้วบอกว่าเป็นเลขคู่หรือคี่
3. เขียนฟังก์ชันหาผลรวมของตัวเลข 1 ถึง n

## 7. เอกสารทางการ

[Python Tutorial](https://docs.python.org/3/tutorial/) · [Downloads](https://www.python.org/downloads/)
