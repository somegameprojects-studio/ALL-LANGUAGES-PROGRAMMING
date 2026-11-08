# คู่มือ PHP ภาษาไทย

PHP เป็นภาษาโปรแกรมฝั่งเซิร์ฟเวอร์ที่นิยมใช้สร้างเว็บไซต์และระบบเว็บ สามารถฝังโค้ดในไฟล์ HTML ได้

## 1. โปรแกรมแรก

บันทึกเป็น `index.php`

```php
<?php
$name = "Mina";
echo "สวัสดี " . $name;
?>
```

`<?php` เริ่มส่วน PHP, ตัวแปรขึ้นต้นด้วย `$` และ `echo` ส่งข้อความออกมา

## 2. วิธีทดลอง

ติดตั้ง PHP จาก [php.net](https://www.php.net/downloads) แล้วใช้ `php index.php` เพื่อรันผ่าน CLI หรือเปิด local development server ด้วย `php -S localhost:8000` และเข้าเว็บในเบราว์เซอร์

## 3. เงื่อนไขและลูป

```php
$score = 80;
if ($score >= 50) {
    echo "ผ่าน";
} else {
    echo "ลองใหม่";
}
for ($i = 1; $i <= 3; $i++) {
    echo $i . PHP_EOL;
}
```

## 4. ฟังก์ชันและอาร์เรย์

```php
function add(int $a, int $b): int {
    return $a + $b;
}
$colors = ["แดง", "เขียว"];
echo add(2, 3);
```

## 5. แนวคิดต่อไป

เรียนรู้ associative arrays, forms, sessions, exceptions, PDO และการป้องกัน SQL injection ด้วย prepared statements

## แบบฝึกหัด

1. สร้างฟังก์ชันแปลงอุณหภูมิ
2. วนแสดงสินค้าในอาร์เรย์
3. สร้างฟอร์มรับชื่อและแสดงผลอย่างปลอดภัย

## เอกสารทางการ

[PHP Manual](https://www.php.net/manual/en/)
