# คู่มือ Java ภาษาไทย

Java เป็นภาษาโปรแกรมที่ทำงานบน Java Virtual Machine (JVM) นิยมใช้กับระบบองค์กร แอปพลิเคชัน และบริการฝั่งเซิร์ฟเวอร์

## 1. โปรแกรมแรก

บันทึกเป็น `Main.java`

```java
public class Main {
    public static void main(String[] args) {
        String name = "Mina";
        System.out.println("สวัสดี " + name);
    }
}
```

ชื่อไฟล์ต้องตรงกับชื่อ public class ในตัวอย่างนี้ ใช้ JDK เพื่อคอมไพล์และรันด้วย `javac Main.java` และ `java Main`

## 2. ชนิดข้อมูลและเงื่อนไข

```java
int score = 65;
if (score >= 50) {
    System.out.println("ผ่าน");
} else {
    System.out.println("ลองใหม่");
}
```

## 3. ลูปและเมธอด

```java
static int add(int a, int b) {
    return a + b;
}
for (int i = 1; i <= 3; i++) {
    System.out.println(i);
}
```

เมธอดคือชุดคำสั่งที่ประกาศไว้ภายในคลาสและเรียกใช้งานได้

## 4. แนวคิดต่อไป

เรียนรู้ class, object, interface, collections, exception และการจัดการโปรเจกต์ด้วย Maven หรือ Gradle

## แบบฝึกหัด

1. สร้างเมธอดตรวจเลขคู่
2. รวมค่าจากอาร์เรย์
3. สร้างคลาส Student ที่มีชื่อและคะแนน

## เอกสารทางการ

[Dev.java](https://dev.java/learn/) · [Java Downloads](https://www.oracle.com/java/technologies/downloads/)
