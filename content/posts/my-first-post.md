---
title: "Giới thiệu về Java"

date : 2024-12-26T20:46:34+07:00
draft: false    
---
Java là một trong những ngôn ngữ lập trình phổ biến nhất trên thế giới, được phát triển bởi Sun Microsystems (nay là Oracle). Java đã ra đời vào năm 1995 và từ đó đến nay đã trở thành ngôn ngữ lập trình hàng đầu trong nhiều lĩnh vực, đặc biệt là trong phát triển ứng dụng web, ứng dụng di động, và hệ thống doanh nghiệp.

### Tại sao chọn Java?

1. **Khả năng di động**: Java được thiết kế với nguyên lý "Viết một lần, chạy mọi nơi". Điều này có nghĩa là một ứng dụng Java có thể chạy trên bất kỳ nền tảng nào có Java Virtual Machine (JVM), giúp các ứng dụng Java có tính di động cao.
   
2. **Ngôn ngữ hướng đối tượng**: Java sử dụng mô hình lập trình hướng đối tượng (OOP), giúp tổ chức mã nguồn một cách hiệu quả và dễ dàng bảo trì.

3. **Thư viện phong phú**: Java cung cấp một lượng lớn các thư viện và API hỗ trợ các tác vụ khác nhau, từ xử lý tệp tin, kết nối cơ sở dữ liệu đến xây dựng giao diện người dùng.

### Các khái niệm cơ bản trong Java

- **Biến**: Là nơi lưu trữ dữ liệu trong bộ nhớ.
- **Lớp (Class)**: Là khuôn mẫu để tạo đối tượng trong Java.
- **Đối tượng (Object)**: Là thể hiện của một lớp.
- **Phương thức (Method)**: Là các hàm hoặc hành động mà đối tượng có thể thực hiện.

### Ví dụ đơn giản về chương trình Java

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}