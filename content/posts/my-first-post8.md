---
date : 2024-12-26T21:42:54+07:00
draft : false
title : 'Lập trình Java nâng cao'
---
# Lập trình Java nâng cao

Lập trình Java không chỉ đơn giản là việc nắm vững các cú pháp cơ bản, mà còn bao gồm việc hiểu và sử dụng các khái niệm nâng cao để xây dựng các ứng dụng phức tạp và hiệu quả. Bài viết này sẽ giới thiệu một số chủ đề nâng cao trong Java giúp bạn nâng cao kỹ năng lập trình của mình.

## 1. Kế thừa (Inheritance) và Đa hình (Polymorphism)

### Kế thừa
Kế thừa là một trong những tính năng quan trọng nhất trong lập trình hướng đối tượng. Nó cho phép bạn tái sử dụng mã của lớp cha mà không cần phải viết lại. Lớp con có thể kế thừa các thuộc tính và phương thức của lớp cha.

**Ví dụ về kế thừa:**

```java
class Animal {
    public void sound() {
        System.out.println("Chúng tôi phát ra âm thanh.");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Gâu gâu!");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        myDog.sound(); // Kết quả: Gâu gâu!
    }
}
```
###  Đa hình
Đa hình cho phép bạn sử dụng một phương thức hoặc một đối tượng của lớp cha như thể nó là đối tượng của lớp con. Điều này giúp tăng tính linh hoạt và mở rộng mã nguồn.

Ví dụ về đa hình:

```java
class Shape {
    public void draw() {
        System.out.println("Vẽ hình cơ bản.");
    }
}

class Circle extends Shape {
    @Override
    public void draw() {
        System.out.println("Vẽ hình tròn.");
    }
}

class Rectangle extends Shape {
    @Override
    public void draw() {
        System.out.println("Vẽ hình chữ nhật.");
    }
}

public class Main {
    public static void main(String[] args) {
        Shape myShape = new Circle();
        myShape.draw(); // Kết quả: Vẽ hình tròn.

        myShape = new Rectangle();
        myShape.draw(); // Kết quả: Vẽ hình chữ nhật.
    }
}
```
## 2. Xử lý ngoại lệ (Exception Handling)
Java cung cấp một cơ chế mạnh mẽ để xử lý các lỗi trong quá trình thực thi thông qua khối try-catch. Điều này giúp ứng dụng của bạn trở nên ổn định hơn và dễ dàng kiểm soát lỗi.

Ví dụ về xử lý ngoại lệ:

```java
public class Main {
    public static void main(String[] args) {
        try {
            int result = 10 / 0; // Đây sẽ gây ra lỗi chia cho 0
        } catch (ArithmeticException e) {
            System.out.println("Lỗi: " + e.getMessage());
        } finally {
            System.out.println("Khối finally luôn được thực thi.");
        }
    }
}
```
## 3. Các lớp trừu tượng và giao diện (Abstract Classes & Interfaces)
Trong Java, lớp trừu tượng và giao diện giúp bạn tạo ra các mẫu thiết kế linh hoạt và có thể mở rộng. Chúng giúp định nghĩa các phương thức mà các lớp con phải triển khai mà không cần lo lắng về cách triển khai cụ thể.

### Lớp trừu tượng
Một lớp trừu tượng là lớp không thể được khởi tạo trực tiếp và thường chứa các phương thức trừu tượng mà các lớp con cần triển khai.

```java
abstract class Animal {
    public abstract void sound();

    public void eat() {
        System.out.println("Động vật ăn thức ăn.");
    }
}

class Dog extends Animal {
    @Override
    public void sound() {
        System.out.println("Gâu gâu!");
    }
}
```
### Giao diện
Giao diện trong Java là một loại lớp trừu tượng chỉ có phương thức mà không có thân phương thức. Lớp con cần phải triển khai tất cả các phương thức của giao diện.

```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    @Override
    public void sound() {
        System.out.println("Gâu gâu!");
    }
}
```
## 4. Bộ sưu tập (Collections)
Java cung cấp một bộ công cụ phong phú để làm việc với dữ liệu không xác định số lượng, chẳng hạn như các lớp trong package java.util như ArrayList, HashMap, HashSet, v.v.

Ví dụ sử dụng ArrayList:
```java
import java.util.ArrayList;

public class Main {
    public static void main(String[] args) {
        ArrayList<String> list = new ArrayList<>();
        list.add("Java");
        list.add("Python");
        list.add("C++");

        for (String language : list) {
            System.out.println(language);
        }
    }
}
```
Ví dụ sử dụng HashMap:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, String> map = new HashMap<>();
        map.put("Java", "Ngôn ngữ lập trình hướng đối tượng.");
        map.put("Python", "Ngôn ngữ lập trình đơn giản và dễ học.");

        System.out.println(map.get("Java"));
    }
}
```
## 5. Đa luồng (Multithreading)
Java hỗ trợ đa luồng, cho phép bạn thực hiện nhiều công việc đồng thời. Điều này rất hữu ích trong các ứng dụng yêu cầu xử lý đồng thời, chẳng hạn như các máy chủ web, ứng dụng giao dịch, v.v.

Ví dụ về đa luồng:
```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Đang chạy trong luồng " + Thread.currentThread().getId());
    }
}

public class Main {
    public static void main(String[] args) {
        MyThread thread1 = new MyThread();
        thread1.start();

        MyThread thread2 = new MyThread();
        thread2.start();
    }
}
```
## 6. Streams và Lambda Expressions
Từ Java 8, Java đã hỗ trợ Streams và Lambda Expressions, giúp mã nguồn ngắn gọn hơn và dễ dàng xử lý các tập dữ liệu.

Ví dụ về Stream và Lambda:
```java

import java.util.Arrays;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        List<String> languages = Arrays.asList("Java", "Python", "C++", "JavaScript");
        
        languages.stream()
                 .filter(language -> language.startsWith("J"))
                 .forEach(System.out::println);
    }
}
```
- **Giải thích**:
- **`stream()`**: Chuyển đổi danh sách thành Stream.
- **`filter()`**: Lọc các phần tử bắt đầu bằng chữ "J".
- **`forEach()`**: In các phần tử còn lại.

## Kết luận
Lập trình Java nâng cao giúp bạn phát triển các ứng dụng mạnh mẽ, hiệu quả và dễ mở rộng. Bằng cách nắm vững các khái niệm như kế thừa, đa hình, xử lý ngoại lệ, và các công nghệ mới như Streams và Lambda, bạn sẽ có thể xây dựng các ứng dụng phức tạp và tối ưu hơn.

Hãy tiếp tục học hỏi và thực hành để trở thành một lập trình viên Java giỏi và có thể phát triển các ứng dụng chuyên nghiệp!