# คู่มือ C++ ภาษาไทย

C++ เป็นภาษาโปรแกรมแบบคอมไพล์ที่รองรับทั้งการเขียนแบบ procedural และ object-oriented ใช้ทำซอฟต์แวร์ เกม และระบบประสิทธิภาพสูง

## 1. โปรแกรมแรก

บันทึกเป็น `main.cpp`

```cpp
#include <iostream>
#include <string>

int main() {
    std::string name = "Mina";
    std::cout << "สวัสดี " << name << '\\n';
    return 0;
}
```

`#include` เรียกใช้ไลบรารี, `std::string` เก็บข้อความ และ `std::cout` แสดงผล

## 2. คอมไพล์

ใช้ compiler ที่รองรับ C++ เช่น GCC, Clang หรือ MSVC อ่านวิธีใช้ตามระบบของตนเอง ตัวอย่าง GCC: `g++ main.cpp -std=c++17 -o app` แล้วรันไฟล์ app

## 3. เงื่อนไขและลูป

```cpp
int score = 80;
if (score >= 50) std::cout << "ผ่าน\\n";
for (int i = 1; i <= 3; ++i) std::cout << i << '\\n';
```

## 4. ฟังก์ชันและ vector

```cpp
#include <vector>
int sum(const std::vector<int>& values) {
    int total = 0;
    for (int value : values) total += value;
    return total;
}
```

## 5. แนวคิดต่อไป

เรียนรู้ reference, pointer, class, template, STL และการจัดการหน่วยความจำอย่างปลอดภัยตามลำดับ

## แบบฝึกหัด

1. สร้างฟังก์ชันหาค่าเฉลี่ย
2. หาค่าสูงสุดใน vector
3. สร้าง class สำหรับเก็บข้อมูลหนังสือ

## เอกสารทางการ

[cppreference](https://en.cppreference.com/w/) · [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines)
