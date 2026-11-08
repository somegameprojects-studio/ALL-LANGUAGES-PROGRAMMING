# Hello, World! — Working Examples

These examples show the smallest useful program or document for a selection of languages and technologies in this repository. They are starting points, not a claim that every tool uses a \`print()\` function.

> **Before running:** install the language's official runtime/compiler and check its current documentation. Commands can vary by operating system and toolchain version.

## Programming languages

### Python

\`\`\`python
print("Hello, World!")
\`\`\`
Run: \`python hello.py\`

### JavaScript

\`\`\`javascript
console.log("Hello, World!");
\`\`\`
Run: \`node hello.js\`

### TypeScript

\`\`\`typescript
const message: string = "Hello, World!";
console.log(message);
\`\`\`
Run with a TypeScript runtime such as \`tsx hello.ts\`, or compile with the TypeScript compiler.

### C

\`\`\`c
#include <stdio.h>

int main(void) {
    printf("Hello, World!\\n");
    return 0;
}
\`\`\`
Compile: \`cc hello.c -o hello\` · Run: \`./hello\`

### C++

\`\`\`cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!\\n";
    return 0;
}
\`\`\`
Compile: \`c++ hello.cpp -o hello\` · Run: \`./hello\`

### C#

\`\`\`csharp
Console.WriteLine("Hello, World!");
\`\`\`
Run in a .NET project: \`dotnet run\`

### Java

\`\`\`java
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
\`\`\`
Run: \`javac Hello.java && java Hello\`

### Go

\`\`\`go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
\`\`\`
Run: \`go run hello.go\`

### Rust

\`\`\`rust
fn main() {
    println!("Hello, World!");
}
\`\`\`
Run: \`rustc hello.rs && ./hello\`

### PHP

\`\`\`php
<?php
echo "Hello, World!\\n";
\`\`\`
Run: \`php hello.php\`

### Ruby

\`\`\`ruby
puts "Hello, World!"
\`\`\`
Run: \`ruby hello.rb\`

### Lua

\`\`\`lua
print("Hello, World!")
\`\`\`
Run: \`lua hello.lua\`

### Swift

\`\`\`swift
print("Hello, World!")
\`\`\`
Run: \`swift hello.swift\`

### Kotlin

\`\`\`kotlin
fun main() {
    println("Hello, World!")
}
\`\`\`
Run with the Kotlin compiler or a Kotlin project.

### Dart

\`\`\`dart
void main() {
  print('Hello, World!');
}
\`\`\`
Run: \`dart run hello.dart\`

### Bash

\`\`\`bash
#!/usr/bin/env bash
printf '%s\\n' 'Hello, World!'
\`\`\`
Run: \`bash hello.sh\`

### PowerShell

\`\`\`powershell
Write-Output "Hello, World!"
\`\`\`
Run: \`pwsh -File hello.ps1\` (or \`powershell -File hello.ps1\` on Windows PowerShell).

### Perl

\`\`\`perl
use strict;
use warnings;

print "Hello, World!\\n";
\`\`\`
Run: \`perl hello.pl\`

### R

\`\`\`r
print("Hello, World!")
\`\`\`
Run: \`Rscript hello.R\`

### Julia

\`\`\`julia
println("Hello, World!")
\`\`\`
Run: \`julia hello.jl\`

### Scala

\`\`\`scala
object Hello {
  def main(args: Array[String]): Unit =
    println("Hello, World!")
}
\`\`\`
Run with the Scala CLI: \`scala Hello.scala\`

### Elixir

\`\`\`elixir
IO.puts("Hello, World!")
\`\`\`
Run: \`elixir hello.exs\`

### Haskell

\`\`\`haskell
main :: IO ()
main = putStrLn "Hello, World!"
\`\`\`
Run with GHC: \`runghc hello.hs\`

### Clojure

\`\`\`clojure
(println "Hello, World!")
\`\`\`
Run with the Clojure CLI: \`clojure -M hello.clj\` (project setup may vary).

### F#

\`\`\`fsharp
printfn "Hello, World!"
\`\`\`
Run as a script: \`dotnet fsi hello.fsx\`

### Objective-C

\`\`\`objective-c
#import <Foundation/Foundation.h>

int main(void) {
    @autoreleasepool {
        NSLog(@"Hello, World!");
    }
    return 0;
}
\`\`\`
Compile on macOS with the Apple toolchain: \`clang hello.m -framework Foundation -o hello\`.

### Assembly (NASM, x86-64 Linux)

\`\`\`asm
section .data
    message db "Hello, World!", 10
    length equ $ - message

section .text
    global _start

_start:
    mov eax, 1
    mov edi, 1
    mov rsi, message
    mov edx, length
    syscall

    mov eax, 60
    xor edi, edi
    syscall
\`\`\`
This is a Linux x86-64 system-call example; assemble/link commands depend on the installed NASM and linker.

## Markup, query, and configuration examples

These formats are not all general-purpose programming languages. They describe documents, data, queries, or build instructions.

### HTML

\`\`\`html
<!doctype html>
<html lang="en">
  <head><meta charset="utf-8"><title>Hello</title></head>
  <body><h1>Hello, World!</h1></body>
</html>
\`\`\`
Open the file in a web browser.

### CSS

\`\`\`css
body {
  font-family: system-ui, sans-serif;
}

h1::before {
  content: "Hello, ";
}
\`\`\`
CSS styles HTML; it does not run as a standalone print program.

### SQL

\`\`\`sql
SELECT 'Hello, World!' AS message;
\`\`\`
Run in a compatible SQL database or SQL console.

### GraphQL

\`\`\`graphql
query Greeting {
  greeting
}
\`\`\`
This is a query document; it needs a GraphQL server that exposes a \`greeting\` field.

### JSON

\`\`\`json
{
  "message": "Hello, World!"
}
\`\`\`
JSON is a data format, not executable code.

### YAML

\`\`\`yaml
message: Hello, World!
\`\`\`
YAML is a data-serialization format, not executable code.

### XML

\`\`\`xml
<?xml version="1.0" encoding="UTF-8"?>
<message>Hello, World!</message>
\`\`\`
XML describes structured data; an application must read or display it.

### Makefile

\`\`\`makefile
.PHONY: hello
hello:
\t@echo "Hello, World!"
\`\`\`
Run: \`make hello\`

### Dockerfile

\`\`\`dockerfile
FROM alpine:latest
CMD ["sh", "-c", "echo 'Hello, World!'"]
\`\`\`
Build and run using Docker: \`docker build -t hello-example . && docker run --rm hello-example\`.

### Solidity

\`\`\`solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Greeting {
    function message() external pure returns (string memory) {
        return "Hello, World!";
    }
}
\`\`\`
This is a smart contract example. Compile and test it with a Solidity development tool; deploying requires a compatible blockchain environment.

## Next steps

For each language, expand the matching \`languages/<language>/\` guide with:
1. Installation and version information.
2. Variables, data types, operators, and control flow.
3. Functions and reusable code.
4. Input/output and error handling.
5. Data structures, modules, and packages.
6. A small practical project.

Contributions should be tested and should link to the language's official documentation.


---

# อธิบายแบบง่ายมาก ๆ 🧸

ไม่ต้องกลัวโค้ดนะ คิดซะว่าเราเป็นคนสั่งงานหุ่นยนต์ตัวหนึ่ง เราพิมพ์คำสั่งอะไรให้มัน มันก็ทำตามนั้น

## ก่อนเริ่ม: Hello, World! คืออะไร?

คำว่า `Hello, World!` แปลว่า “สวัสดีชาวโลก”

เวลาเราเขียนโปรแกรมครั้งแรก เรามักสั่งให้คอมพิวเตอร์พูดประโยคนี้ เหมือนเราทักทายคอมพิวเตอร์ว่า “ฮัลโหล ได้ยินไหม?”

## คำสั่งแสดงข้อความของแต่ละภาษา

### Python

```python
print("Hello, World!")
```

- `print` แปลว่า เอาข้อความออกมาโชว์ให้ดู
- วงเล็บ `()` คือช่องใส่สิ่งที่เราอยากให้โชว์
- เครื่องหมายคำพูด `"` บอกว่า ข้างในนี้เป็นข้อความนะ
- คอมพิวเตอร์จึงแสดงคำว่า `Hello, World!` ออกมา

นึกภาพว่าเราบอกเพื่อนว่า “พูดคำนี้ให้หน่อย” แล้วเพื่อนก็พูดตาม

### JavaScript

```javascript
console.log("Hello, World!");
```

- `console` คือหน้าต่างที่เอาไว้ดูข้อความจากโปรแกรม
- `log` คือการเขียนข้อความลงไปในหน้าต่างนั้น
- ข้อความในวงเล็บคือสิ่งที่เราอยากให้แสดง
- เครื่องหมาย `;` ใช้ปิดคำสั่งใน JavaScript โดยทั่วไป

ผลลัพธ์ก็ยังเป็นคำว่า `Hello, World!` เหมือนเดิม แค่ใช้คำสั่งคนละแบบ

### TypeScript

```typescript
const message: string = "Hello, World!";
console.log(message);
```

- `const` คือการสร้างกล่องเก็บข้อมูลที่เราไม่ตั้งใจเปลี่ยนค่า
- `message` คือชื่อกล่อง
- `string` บอกว่าของในกล่องเป็นข้อความ
- เครื่องหมาย `=` เอาข้อความใส่ลงในกล่อง
- `console.log(message)` สั่งให้เอาของในกล่องออกมาโชว์

เหมือนเราเขียนคำว่า “สวัสดี” ใส่กล่อง แล้วบอกให้คอมพิวเตอร์หยิบมาอ่าน

### C

```c
#include <stdio.h>

int main(void) {
    printf("Hello, World!\\n");
    return 0;
}
```

- `#include <stdio.h>` เรียกเครื่องมือที่มีคำสั่งแสดงข้อความมาใช้
- `int main(void)` คือจุดเริ่มต้นที่โปรแกรม C จะเริ่มทำงาน
- `printf` สั่งให้แสดงข้อความ
- `\\n` บอกให้ขึ้นบรรทัดใหม่
- `return 0` บอกว่าทำงานเสร็จเรียบร้อย
- เครื่องหมาย `{}` ใช้ครอบคำสั่งที่อยู่ในส่วนนี้

### C++

```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!\\n";
    return 0;
}
```

- `#include <iostream>` เรียกเครื่องมือรับและแสดงข้อมูล
- `int main()` เป็นจุดเริ่มทำงาน
- `std::cout` คือเครื่องมือส่งข้อความออกหน้าจอ
- `<<` เหมือนลูกศรส่งข้อความไปให้หน้าจอ
- `return 0` บอกว่าจบงานปกติ

### Java

```java
class Hello {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

- `class Hello` สร้างกลุ่มคำสั่งชื่อ Hello
- `main` คือประตูทางเข้าที่โปรแกรมเริ่มทำงาน
- `System.out.println` สั่งให้แสดงข้อความแล้วขึ้นบรรทัดใหม่
- ข้อความในวงเล็บคือสิ่งที่จะเอาไปโชว์

### Go

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

- `package main` บอกว่านี่คือโปรแกรมที่สามารถเริ่มทำงานได้
- `import "fmt"` เรียกชุดเครื่องมือสำหรับจัดการข้อความ
- `func main()` คือจุดเริ่มต้น
- `fmt.Println` แสดงข้อความแล้วขึ้นบรรทัดใหม่

### Rust

```rust
fn main() {
    println!("Hello, World!");
}
```

- `fn` ใช้สร้างฟังก์ชัน หรือชุดคำสั่ง
- `main` คือชุดคำสั่งหลักที่เริ่มก่อน
- `println!` เป็นคำสั่งสำหรับแสดงข้อความ
- เครื่องหมาย `!` เป็นส่วนหนึ่งของรูปแบบคำสั่งนี้ ไม่ต้องลบออก

### PHP

```php
<?php
echo "Hello, World!\\n";
```

- `<?php` บอกว่าเริ่มเขียนโค้ด PHP แล้วนะ
- `echo` สั่งให้ส่งข้อความออกมา
- ข้อความในเครื่องหมายคำพูดคือสิ่งที่จะแสดง
- `\\n` ใช้ขึ้นบรรทัดใหม่ในข้อความแบบนี้

### Ruby

```ruby
puts "Hello, World!"
```

- `puts` สั่งให้แสดงข้อความ
- ข้อความหลัง `puts` คือสิ่งที่อยากให้โชว์
- จบแล้ว Ruby จะขึ้นบรรทัดใหม่ให้ด้วย

### Lua

```lua
print("Hello, World!")
```

- `print` คือคำสั่งแสดงข้อความ
- วงเล็บใส่ข้อความที่อยากให้แสดง
- สั้น ๆ แค่นี้เอง!

### Swift

```swift
print("Hello, World!")
```

- `print` สั่งให้แสดงข้อความ
- ข้อความในเครื่องหมายคำพูดคือสิ่งที่ต้องการแสดง
- Swift ใช้คำสั่งนี้ได้ตรง ๆ เลย

### Kotlin

```kotlin
fun main() {
    println("Hello, World!")
}
```

- `fun` ใช้สร้างฟังก์ชัน
- `main` คือฟังก์ชันเริ่มต้น
- `println` แสดงข้อความแล้วขึ้นบรรทัดใหม่

### Dart

```dart
void main() {
  print('Hello, World!');
}
```

- `void` หมายถึงฟังก์ชันนี้ไม่ได้ส่งค่ากลับมา
- `main` คือจุดเริ่มโปรแกรม
- `print` เอาข้อความมาแสดง

### Bash

```bash
printf '%s\\n' 'Hello, World!'
```

- `printf` ใช้แสดงข้อความตามรูปแบบที่กำหนด
- `%s` เป็นช่องสำหรับใส่ข้อความ
- ข้อความท้ายคำสั่งจะถูกนำมาใส่ในช่องนั้น
- `\\n` ทำให้ขึ้นบรรทัดใหม่

### PowerShell

```powershell
Write-Output "Hello, World!"
```

- `Write-Output` ส่งข้อความออกมาให้เห็น
- ข้อความในเครื่องหมายคำพูดคือสิ่งที่จะแสดง

### Perl

```perl
use strict;
use warnings;

print "Hello, World!\\n";
```

- `use strict` ช่วยให้เขียนโค้ดอย่างระมัดระวังขึ้น
- `use warnings` เปิดการเตือนเมื่อมีสิ่งน่าสงสัย
- `print` แสดงข้อความ
- `\\n` ขึ้นบรรทัดใหม่

### R

```r
print("Hello, World!")
```

- `print` แสดงข้อมูลออกมา
- ข้อความในวงเล็บคือสิ่งที่อยากให้แสดง

### Julia

```julia
println("Hello, World!")
```

- `println` แสดงข้อความและขึ้นบรรทัดใหม่
- ข้อความในวงเล็บคือสิ่งที่โปรแกรมจะพูด

## แล้วภาษา HTML, CSS, SQL ต่างกันยังไง?

ไม่ใช่ทุกอย่างที่อยู่ในโฟลเดอร์นี้จะเป็นภาษาแบบสั่งให้คอมพิวเตอร์พูดได้ตรง ๆ นะ บางอย่างทำหน้าที่คนละแบบ

### HTML — โครงร่างของหน้าเว็บ

```html
<h1>Hello, World!</h1>
```

คิดว่า HTML เป็นโครงบ้าน คำสั่ง `<h1>` บอกว่า “ข้อความนี้เป็นหัวข้อใหญ่” ส่วน `</h1>` บอกว่าหัวข้อจบตรงนี้

### CSS — เสื้อผ้าและการแต่งตัวของเว็บ

```css
h1 {
  color: blue;
}
```

CSS บอกว่าหัวข้อ `h1` ควรเป็นสีอะไร ตัวอย่างนี้บอกให้หัวข้อเป็นสีน้ำเงิน HTML สร้างหัวข้อ ส่วน CSS แต่งหน้าตาให้มัน

### SQL — คำถามที่เราถามฐานข้อมูล

```sql
SELECT 'Hello, World!' AS message;
```

- `SELECT` แปลว่า ขอเลือกข้อมูลหน่อย
- ข้อความในเครื่องหมายคำพูดคือข้อมูลที่เราขอ
- `AS message` ตั้งชื่อผลลัพธ์ว่า message

เหมือนเราถามกล่องเก็บข้อมูลว่า “ช่วยส่งข้อความนี้กลับมาให้ดูหน่อย”

### JSON — กล่องเก็บข้อมูล

```json
{
  "message": "Hello, World!"
}
```

- `message` คือป้ายชื่อช่องเก็บข้อมูล
- `Hello, World!` คือของที่เก็บอยู่ในช่องนั้น
- JSON เอาไว้เก็บหรือส่งข้อมูล ไม่ได้สั่งให้คอมพิวเตอร์พูดเอง

### YAML — วิธีเขียนข้อมูลอีกแบบ

```yaml
message: Hello, World!
```

บรรทัดนี้หมายถึงมีช่องชื่อ `message` และเก็บข้อความ Hello, World! เอาไว้ YAML ก็เป็นรูปแบบข้อมูลเหมือน JSON แต่เขียนหน้าตาต่างกัน

## จำง่าย ๆ

- `print`, `puts`, `echo`, `console.log` = เอาข้อความมาโชว์
- `"ข้อความ"` = ข้อความที่เราอยากให้คอมพิวเตอร์รู้จัก
- `()` = ช่องใส่ข้อมูลให้คำสั่ง
- `=` = เอาค่ามาใส่ตัวแปร
- `main` = จุดเริ่มต้นของโปรแกรมในหลายภาษา
- HTML = วางโครงหน้าเว็บ
- CSS = แต่งหน้าตาเว็บ
- SQL = ขอข้อมูลจากฐานข้อมูล
- JSON / YAML = รูปแบบเก็บข้อมูล

**จำไว้นิดหนึ่ง:** คอมพิวเตอร์ไม่ได้เดาใจเรา มันทำตามคำสั่งที่เราเขียน ถ้าพิมพ์ผิดนิดเดียว บางทีมันก็ไม่เข้าใจได้ ไม่เป็นไร ค่อย ๆ อ่านทีละบรรทัดแล้วลองแก้ดู!
