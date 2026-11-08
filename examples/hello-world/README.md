# ตัวอย่างแรก: ให้คอมพิวเตอร์แสดงข้อความ

บทนี้สอนแนวคิดแรกของการเขียนโปรแกรม: เราจะสั่งให้คอมพิวเตอร์แสดงข้อความได้อย่างไร

## 1. Hello, World! คืออะไร?

`Hello, World!` แปลว่า “สวัสดีชาวโลก” เป็นข้อความยอดนิยมที่ใช้ทดลองโปรแกรมครั้งแรก เหมือนเราทักคอมพิวเตอร์ว่า “ลองทำงานให้ดูหน่อย”

## 2. ตัวอย่างในภาษาต่าง ๆ

### Python
```python
print("Hello, World!")
```
`print` คือคำสั่งแสดงข้อมูล วงเล็บใส่สิ่งที่อยากแสดง และเครื่องหมายคำพูดบอกว่าสิ่งข้างในเป็นข้อความ

### JavaScript
```javascript
console.log("Hello, World!");
```
`console` คือหน้าต่างดูข้อความ และ `log` คือการเขียนข้อความลงหน้าต่างนั้น

### TypeScript
```typescript
const message: string = "Hello, World!";
console.log(message);
```
`const` สร้างตัวแปร, `message` คือชื่อ, `string` บอกว่าเก็บข้อความ และ `console.log` นำค่ามาแสดง

### C
```c
#include <stdio.h>
int main(void) {
    printf("Hello, World!\\n");
    return 0;
}
```
`#include` เรียกส่วนประกอบที่จำเป็น, `main` เป็นจุดเริ่มต้น, `printf` แสดงข้อความ, `\\n` ขึ้นบรรทัดใหม่ และ `return 0` จบโปรแกรมตามปกติ

### C++
```cpp
#include <iostream>
int main() {
    std::cout << "Hello, World!\\n";
    return 0;
}
```
`std::cout` ใช้ส่งข้อความออกหน้าจอ และ `<<` ส่งข้อมูลไปยังหน้าจอ

### C#
```csharp
Console.WriteLine("Hello, World!");
```
`Console` เป็นเครื่องมือทำงานกับหน้าต่างคอนโซล และ `WriteLine` แสดงข้อความแล้วขึ้นบรรทัดใหม่

### Java
```java
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
`class` ประกาศคลาส, `main` เป็นจุดเริ่มต้น และ `println` แสดงข้อความแล้วขึ้นบรรทัดใหม่

### Go
```go
package main
import "fmt"
func main() {
    fmt.Println("Hello, World!")
}
```
`package main` ระบุโปรแกรมหลัก, `import` เรียกเครื่องมือ และ `fmt.Println` แสดงข้อความ

### Rust
```rust
fn main() {
    println!("Hello, World!");
}
```
`fn` ประกาศฟังก์ชัน, `main` เป็นจุดเริ่มต้น และ `println!` แสดงข้อความ

### PHP
```php
<?php
echo "Hello, World!";
```
`<?php` เริ่มส่วนโค้ด PHP และ `echo` ส่งข้อความออกมา

### Ruby
```ruby
puts "Hello, World!"
```
`puts` แสดงข้อความและขึ้นบรรทัดใหม่

### Lua
```lua
print("Hello, World!")
```
`print` แสดงสิ่งที่อยู่ในวงเล็บ

### Swift
```swift
print("Hello, World!")
```
`print` แสดงข้อความออกทางหน้าต่างผลลัพธ์

### Kotlin
```kotlin
fun main() {
    println("Hello, World!")
}
```
`fun` สร้างฟังก์ชัน และ `println` แสดงข้อความ

### Dart
```dart
void main() {
  print('Hello, World!');
}
```
`main` เป็นจุดเริ่มต้น และ `print` แสดงข้อความ

### Bash
```bash
printf '%s\\n' 'Hello, World!'
```
`printf` แสดงข้อความตามรูปแบบที่กำหนด

### PowerShell
```powershell
Write-Output "Hello, World!"
```
`Write-Output` ส่งข้อความออกมา

### Perl
```perl
print "Hello, World!\\n";
```
`print` แสดงข้อความ และ `\\n` ขึ้นบรรทัดใหม่

### R
```r
print("Hello, World!")
```
`print` แสดงข้อมูล

### Julia
```julia
println("Hello, World!")
```
`println` แสดงข้อความและขึ้นบรรทัดใหม่

### Scala
```scala
object Hello extends App {
  println("Hello, World!")
}
```
`object` สร้าง object และ `println` แสดงข้อความ

### Elixir
```elixir
IO.puts("Hello, World!")
```
`IO.puts` ใช้แสดงข้อความ

### Haskell
```haskell
main = putStrLn "Hello, World!"
```
`main` เป็นจุดเริ่มต้น และ `putStrLn` แสดงข้อความ

### Clojure
```clojure
(println "Hello, World!")
```
คำสั่งอยู่ในวงเล็บ และ `println` แสดงข้อความ

### F#
```fsharp
printfn "Hello, World!"
```
`printfn` แสดงข้อความและขึ้นบรรทัดใหม่

### Objective-C
```objective-c
#import <Foundation/Foundation.h>
int main(void) {
    NSLog(@"Hello, World!");
    return 0;
}
```
`#import` เรียกส่วนประกอบ Foundation และ `NSLog` แสดงข้อความในหน้าต่างบันทึก

### Assembly (NASM บน Linux x86-64)
```asm
section .data
    message db "Hello, World!", 10
    length equ $ - message
section .text
    global _start
_start:
    mov rax, 1
    mov rdi, 1
    mov rsi, message
    mov rdx, length
    syscall
    mov rax, 60
    xor rdi, rdi
    syscall
```
Assembly แตกต่างตามชนิด CPU และระบบปฏิบัติการ ตัวอย่างนี้ใช้กับ NASM บน Linux x86-64 เท่านั้น

## 3. สิ่งที่ไม่ใช่คำสั่ง print

### HTML — วางโครงหน้าเว็บ
```html
<h1>Hello, World!</h1>
```
แท็ก `h1` บอกเบราว์เซอร์ว่านี่คือหัวข้อใหญ่

### CSS — แต่งหน้าตาเว็บ
```css
h1 {
  color: blue;
}
```
เลือกหัวข้อ `h1` แล้วกำหนดสีตัวอักษรเป็นสีน้ำเงิน

### SQL — ขอข้อมูลจากฐานข้อมูล
```sql
SELECT 'Hello, World!' AS message;
```
`SELECT` ขอค่าจากฐานข้อมูล และ `AS` ตั้งชื่อคอลัมน์ผลลัพธ์

### JSON — เก็บข้อมูล
```json
{
  "message": "Hello, World!"
}
```
มีช่องชื่อ `message` ที่เก็บข้อความไว้ JSON เป็นรูปแบบข้อมูล ไม่ใช่คำสั่งให้คอมพิวเตอร์พูด

### YAML — เก็บค่าตั้งค่า
```yaml
message: Hello, World!
```
เก็บข้อความไว้ในช่องชื่อ message เพื่อให้โปรแกรมอื่นอ่านไปใช้

### XML — เก็บข้อมูลด้วยแท็ก
```xml
<message>Hello, World!</message>
```
แท็ก `message` ใช้ครอบข้อมูล

### Dockerfile — บอกวิธีสร้างอิมเมจ
```dockerfile
FROM alpine
CMD ["echo", "Hello, World!"]
```
Docker ใช้ไฟล์นี้เป็นแนวทางสร้างอิมเมจและกำหนดคำสั่งเริ่มต้น

### Solidity — ตัวอย่างสัญญาอัจฉริยะ
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;
contract Hello {
    function message() public pure returns (string memory) {
        return "Hello, World!";
    }
}
```
`contract` ประกาศสัญญา และ `function` ประกาศฟังก์ชัน ตัวอย่างนี้ใช้เพื่อการเรียนรู้ ควรทดลองบนเครือข่ายทดสอบก่อนเสมอ

## 4. ทำไมแต่ละภาษาถึงไม่เหมือนกัน?

เพราะแต่ละภาษาออกแบบมาเพื่อเป้าหมายต่างกัน บางภาษาเขียนโปรแกรม บางอย่างวางโครงหน้าเว็บ บางอย่างค้นหาข้อมูล และบางอย่างเก็บค่าตั้งค่า ให้จำแนวคิดว่าเราส่งอะไรให้เครื่องมือ แล้วเครื่องมือนั้นทำอะไรกับสิ่งที่ส่งไป

## 5. วิธีทดลองด้วยตัวเอง

1. เลือกภาษาเพียงหนึ่งภาษา
2. ติดตั้งเครื่องมือจากแหล่งทางการ
3. สร้างไฟล์ตามนามสกุลที่ถูกต้อง
4. พิมพ์ตัวอย่างด้วยตัวเอง
5. รันตามคำสั่งในคู่มือของเครื่องมือนั้น
6. เปลี่ยนข้อความเป็นคำของตัวเอง
7. สังเกตผลลัพธ์ แล้วลองอธิบายว่าแต่ละบรรทัดทำอะไร

อย่าเพิ่งรีบเรียนทุกภาษาในวันเดียว เรียนทีละภาษาให้เข้าใจวิธีคิดก่อน แล้วค่อยไปภาษาถัดไป
