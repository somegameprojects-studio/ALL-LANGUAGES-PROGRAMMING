# คู่มือ Lua ภาษาไทย

Lua เป็นภาษาโปรแกรมขนาดเล็กที่ฝังลงในโปรแกรมอื่นได้ง่าย นิยมใช้เป็นภาษาสคริปต์ในเกมและระบบปรับแต่งต่าง ๆ

## 1. โปรแกรมแรก

บันทึกเป็น `main.lua`

```lua
local name = "Mina"
print("สวัสดี " .. name)
```

`local` ประกาศตัวแปรในขอบเขตที่กำหนด, `print` แสดงข้อความ และ `..` ใช้ต่อข้อความ

## 2. วิธีรัน

ติดตั้ง Lua จาก [lua.org](https://www.lua.org/) หรือใช้ runtime ที่โปรแกรมเป้าหมายจัดเตรียม แล้วรันด้วย `lua main.lua`

## 3. เงื่อนไขและลูป

```lua
local score = 70
if score >= 50 then
    print("ผ่าน")
else
    print("ลองใหม่")
end

for i = 1, 3 do
    print(i)
end
```

## 4. ฟังก์ชันและตาราง

```lua
local function add(a, b)
    return a + b
end
local colors = {"red", "green", "blue"}
print(add(2, 3), colors[1])
```

ตาราง (table) เป็นโครงสร้างข้อมูลหลัก ใช้ทำหน้าที่คล้ายอาร์เรย์และ map ได้

## 5. แบบฝึกหัด

1. สร้างฟังก์ชันคูณเลข
2. วนแสดงสมาชิกใน table
3. ทำเกมทายตัวเลขแบบง่าย

## เอกสารทางการ

[Lua 5.4 Reference Manual](https://www.lua.org/manual/5.4/)
