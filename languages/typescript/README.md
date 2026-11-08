# คู่มือ TypeScript ภาษาไทย

TypeScript ต่อยอดจาก JavaScript โดยเพิ่มระบบชนิดข้อมูล (type) เพื่อช่วยตรวจข้อผิดพลาดก่อนรัน และคอมไพล์เป็น JavaScript

## 1. ตัวอย่างแรก

```ts
const username: string = "Mina";
let score: number = 80;
score += 5;
console.log(username, score);
```

`string` คือข้อความ และ `number` คือตัวเลข หากกำหนดค่าผิดชนิด ตัวตรวจ TypeScript จะแจ้งเตือน

## 2. ฟังก์ชัน

```ts
function add(a: number, b: number): number {
  return a + b;
}
console.log(add(2, 3));
```

ชนิดหลังวงเล็บคือชนิดค่าที่ฟังก์ชันส่งกลับ

## 3. Object และ Interface

```ts
interface User {
  name: string;
  active: boolean;
}
const user: User = { name: "Mina", active: true };
```

## 4. วิธีทดลอง

ติดตั้ง Node.js และ TypeScript ตาม [คู่มือทางการ](https://www.typescriptlang.org/download/) จากนั้นใช้ `tsc main.ts` เพื่อสร้าง JavaScript แล้วรันไฟล์ผลลัพธ์ด้วย Node.js หรือใช้เครื่องมือพัฒนาที่ตั้งค่า TypeScript ไว้แล้ว

## 5. แบบฝึกหัด

1. สร้างฟังก์ชันคูณเลขที่รับ number สองค่า
2. สร้าง interface สำหรับสินค้า
3. เขียนฟังก์ชันที่รับอาร์เรย์ตัวเลขและคืนค่าผลรวม

## เอกสารทางการ

[TypeScript Handbook](https://www.typescriptlang.org/docs/)
