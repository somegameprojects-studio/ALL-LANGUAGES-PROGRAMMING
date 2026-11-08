# คู่มือ JavaScript ภาษาไทย

JavaScript เป็นภาษาโปรแกรมที่ใช้เพิ่มการโต้ตอบบนเว็บไซต์ และยังทำงานฝั่งเซิร์ฟเวอร์ได้ผ่าน runtime เช่น Node.js

## 1. ทดลองบนเว็บ

เปิด Developer Tools ของเบราว์เซอร์ เลือก Console แล้วพิมพ์ `console.log("Hello")` หรือสร้างไฟล์ `main.js` แล้วรันด้วย Node.js ด้วยคำสั่ง `node main.js`

## 2. ตัวแปรและชนิดข้อมูล

```js
const siteName = "CodeAtlas";
let visits = 0;
visits = visits + 1;
console.log(siteName, visits);
```

ใช้ `const` เมื่อไม่ต้องกำหนดค่าใหม่ และ `let` เมื่อค่าจะเปลี่ยนได้

## 3. เงื่อนไขและลูป

```js
const score = 72;
if (score >= 50) {
  console.log("ผ่าน");
} else {
  console.log("ลองใหม่");
}
for (let i = 1; i <= 3; i++) {
  console.log(i);
}
```

## 4. ฟังก์ชันและอาร์เรย์

```js
function greet(name) {
  return "สวัสดี " + name;
}
const colors = ["แดง", "เขียว", "น้ำเงิน"];
console.log(greet("Mina"));
colors.forEach(color => console.log(color));
```

## 5. ใช้กับหน้าเว็บ

JavaScript เข้าถึง DOM เพื่ออ่านหรือเปลี่ยนเนื้อหาเว็บได้ เช่น `document.querySelector("h1").textContent = "สวัสดี"` ควรตรวจว่า element มีอยู่ก่อนใช้งาน

## 6. ข้อผิดพลาดที่พบบ่อย

- `ReferenceError`: ใช้ตัวแปรที่ไม่มีหรืออยู่นอกขอบเขต
- `TypeError`: เรียกใช้ค่าด้วยวิธีที่ไม่รองรับ
- `SyntaxError`: รูปแบบโค้ดไม่ถูกต้อง

## 7. แบบฝึกหัด

1. สร้างฟังก์ชันบวกเลขสองจำนวน
2. กรองเลขคู่จากอาร์เรย์
3. สร้างปุ่มบนเว็บที่คลิกแล้วเปลี่ยนข้อความ

## เอกสารทางการ

[MDN JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide) · [Node.js](https://nodejs.org/)
