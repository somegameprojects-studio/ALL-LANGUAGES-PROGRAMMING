# คู่มือ Rust ภาษาไทย

Rust เป็นภาษาโปรแกรมแบบคอมไพล์ที่เน้นความปลอดภัยของหน่วยความจำและประสิทธิภาพ โดยใช้แนวคิด ownership และ borrowing

## 1. โปรแกรมแรก

สร้างโปรเจกต์ด้วย `cargo new hello_rust` แล้วแก้ไฟล์ `src/main.rs`

```rust
fn main() {
    let name = "Mina";
    println!("สวัสดี {name}");
}
```

`fn main()` คือจุดเริ่มต้น, `let` ประกาศตัวแปร และ `println!` เป็น macro แสดงข้อความ

## 2. วิธีรัน

ติดตั้ง Rust ผ่าน [rustup](https://rustup.rs/) แล้วเข้าโฟลเดอร์โปรเจกต์ ใช้ `cargo run` เพื่อ build และรัน

## 3. เงื่อนไขและลูป

```rust
let score = 75;
if score >= 50 { println!("ผ่าน"); } else { println!("ลองใหม่"); }
for number in 1..=3 { println!("{number}"); }
```

## 4. ฟังก์ชันและ ownership

```rust
fn add(a: i32, b: i32) -> i32 {
    a + b
}
```

Rust ตรวจการยืมและการเป็นเจ้าของข้อมูลในช่วง compile time เพื่อช่วยป้องกันข้อผิดพลาดด้านหน่วยความจำ

## 5. แนวคิดต่อไป

เรียนรู้ String, Vec, Option, Result, struct, enum, borrowing และ pattern matching

## แบบฝึกหัด

1. เขียนฟังก์ชันตรวจเลขคู่
2. หาผลรวมของ vector
3. ใช้ Result จัดการกรณีแปลงข้อความเป็นตัวเลขไม่สำเร็จ

## เอกสารทางการ

[The Rust Book](https://doc.rust-lang.org/book/) · [Rust By Example](https://doc.rust-lang.org/rust-by-example/)
