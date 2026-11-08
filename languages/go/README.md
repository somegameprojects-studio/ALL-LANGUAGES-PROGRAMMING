# คู่มือ Go ภาษาไทย

Go (Golang) เป็นภาษาโปรแกรมแบบคอมไพล์ ออกแบบให้เรียบง่ายและเหมาะกับบริการเครือข่าย โปรแกรมฝั่งเซิร์ฟเวอร์ และเครื่องมือ command-line

## 1. โปรแกรมแรก

บันทึกเป็น `main.go`

```go
package main
import "fmt"

func main() {
    name := "Mina"
    fmt.Println("สวัสดี", name)
}
```

`package main` ระบุโปรแกรมที่สร้างเป็น executable, `import` นำแพ็กเกจมาใช้ และ `:=` ให้ Go อนุมานชนิดตัวแปร

## 2. วิธีรัน

ติดตั้ง Go จาก [เว็บไซต์ทางการ](https://go.dev/dl/) แล้วใช้ `go run main.go` เพื่อทดลอง หรือ `go build` เพื่อสร้างไฟล์โปรแกรม

## 3. เงื่อนไขและลูป

```go
score := 80
if score >= 50 {
    fmt.Println("ผ่าน")
}
for i := 1; i <= 3; i++ {
    fmt.Println(i)
}
```

## 4. ฟังก์ชัน

```go
func add(a int, b int) int {
    return a + b
}
```

## 5. แนวคิดต่อไป

เรียนรู้ slice, map, struct, interface, error และ goroutine โดยตรวจการจัดการ error ที่คืนค่าจากฟังก์ชันเสมอ

## แบบฝึกหัด

1. สร้างฟังก์ชันหาผลรวม
2. นับจำนวนคำในข้อความ
3. สร้าง struct สำหรับสินค้า

## เอกสารทางการ

[The Go Tour](https://go.dev/tour/) · [Go Documentation](https://go.dev/doc/)
