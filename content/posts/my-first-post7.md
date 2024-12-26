---
date : 2024-12-26T21:33:00+07:00
draft : false
title : 'Lập trình Java cơ bản'
---

# Lập trình Java cơ bản

Java là một trong những ngôn ngữ lập trình phổ biến và mạnh mẽ nhất hiện nay, được sử dụng rộng rãi trong phát triển phần mềm, ứng dụng di động (Android), và các hệ thống lớn. Nếu bạn là người mới bắt đầu học lập trình, Java là một lựa chọn tuyệt vời. Bài viết này sẽ cung cấp cho bạn những kiến thức cơ bản về lập trình Java.

## 1. Cài đặt Java

Trước khi bắt đầu lập trình Java, bạn cần cài đặt Java Development Kit (JDK). JDK là bộ công cụ cần thiết để phát triển và biên dịch các chương trình Java.

### Các bước cài đặt:
1. Tải JDK từ trang chính thức của Oracle: [Tải JDK](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html).
2. Cài đặt JDK vào máy tính của bạn và thêm `JAVA_HOME` vào biến môi trường (Environment Variables).
3. Kiểm tra cài đặt bằng cách mở Command Prompt (Windows) hoặc Terminal (Mac/Linux) và chạy lệnh sau:
   ```bash
   java -version
   ```
Nếu Java đã được cài đặt thành công, bạn sẽ thấy thông tin phiên bản Java.

## 2. Cấu trúc một chương trình Java
Một chương trình Java cơ bản bao gồm các phần chính: khai báo lớp (class), phương thức chính (main method), và các câu lệnh thực thi. Dưới đây là ví dụ về một chương trình Java đơn giản:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Chào thế giới!");
    }
}
```
## 3. Các kiểu dữ liệu trong Java
Java là ngôn ngữ lập trình kiểu dữ liệu tĩnh, có nghĩa là bạn phải chỉ định kiểu dữ liệu khi khai báo biến. Các kiểu dữ liệu cơ bản trong Java bao gồm:

- **`int`**: Kiểu số nguyên (ví dụ: int age = 30;).
- **`double`**: Kiểu số thực (ví dụ: double price = 10.99;).
- **`boolean`**: Kiểu giá trị logic (ví dụ: boolean isActive = true;).
- **`char`**: Kiểu ký tự (ví dụ: char grade = 'A';).
- **`String`**: Kiểu chuỗi (ví dụ: String name = "John";).
## 4. Câu lệnh điều kiện (if-else)
Câu lệnh điều kiện cho phép bạn thực hiện các quyết định dựa trên điều kiện. Dưới đây là ví dụ về cách sử dụng **`if-else `**trong Java:

```java
int age = 20;
if (age >= 18) {
    System.out.println("Bạn đủ tuổi trưởng thành.");
} else {
    System.out.println("Bạn chưa đủ tuổi trưởng thành.");
}
```
## 5. Vòng lặp (Loops)
Java hỗ trợ ba loại vòng lặp cơ bản: for, while, và do-while.

-   Vòng lặp for:
```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```
-   Vòng lặp while:
```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
```
-   Vòng lặp do-while:
```java

int i = 0;
do {
    System.out.println(i);
    i++;
} while (i < 5);
```
## 6. Hàm (Methods)
Hàm (hay phương thức) trong Java là một khối mã thực hiện một tác vụ cụ thể. Bạn có thể khai báo hàm bằng cách sử dụng cú pháp sau:

```java

public class Calculator {
    public static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int result = add(5, 3);
        System.out.println("Kết quả là: " + result);
    }
}
```
## 7. Lớp và Đối tượng (Classes and Objects)
Trong Java, mọi thứ đều là đối tượng. Để sử dụng đối tượng, bạn cần tạo một lớp (class), trong đó định nghĩa các thuộc tính và phương thức của đối tượng.

Ví dụ:
```java
class Dog {
    String name;
    int age;

    public void bark() {
        System.out.println(name + " đang sủa!");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog dog1 = new Dog();
        dog1.name = "Buddy";
        dog1.age = 3;
        dog1.bark(); // Kết quả sẽ là 'Buddy đang sủa!'
    }
}
```
## Kết luận
Java là một ngôn ngữ lập trình mạnh mẽ và dễ học, phù hợp cho cả người mới bắt đầu và các lập trình viên có kinh nghiệm. Bằng cách nắm vững các cú pháp cơ bản và thực hành liên tục, bạn sẽ trở thành một lập trình viên Java giỏi.

Hãy tiếp tục tìm hiểu các chủ đề nâng cao hơn như kế thừa, đa hình, và xử lý ngoại lệ để phát triển kỹ năng lập trình của mình!
