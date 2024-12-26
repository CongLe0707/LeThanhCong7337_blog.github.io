---
date : 2024-12-26T21:07:23+07:00
draft: false   
title : 'Hướng dẫn cách cài đặt Java'
---
## Hướng dẫn cách cài đặt Java

Java là một trong những ngôn ngữ lập trình phổ biến nhất, được sử dụng rộng rãi trong phát triển ứng dụng di động (Android), web, và phần mềm doanh nghiệp. Dưới đây là hướng dẫn chi tiết về cách cài đặt Java Development Kit (JDK) trên các hệ điều hành phổ biến.

### 1. Cài đặt Java trên Windows

Để cài đặt Java trên Windows, bạn có thể thực hiện các bước sau:

#### Bước 1: Tải xuống JDK
- Truy cập vào trang tải Java chính thức của Oracle tại [Java Downloads](https://www.oracle.com/java/technologies/javase-downloads.html).
- Chọn phiên bản JDK (Java Development Kit) phù hợp với hệ điều hành của bạn và tải về.

#### Bước 2: Cài đặt JDK
- Sau khi tải về, chạy tệp cài đặt `.exe`.
- Làm theo hướng dẫn trên màn hình để cài đặt Java.
- Lưu ý rằng bạn nên ghi nhớ đường dẫn cài đặt, thường là `C:\Program Files\Java\jdk-version`.

#### Bước 3: Cấu hình biến môi trường (Environment Variables)
- Mở "Control Panel" và tìm đến "System and Security" > "System".
- Chọn "Advanced system settings" và nhấp vào "Environment Variables".
- Trong phần "System variables", nhấn vào "New" để tạo một biến môi trường mới:
  - Tên biến: `JAVA_HOME`
  - Giá trị biến: Đường dẫn cài đặt JDK của bạn (ví dụ: `C:\Program Files\Java\jdk-17`).
- Tiếp theo, trong phần "System variables", tìm và chọn biến `Path`, sau đó nhấn "Edit".
- Thêm đường dẫn `bin` vào cuối giá trị của `Path`. Ví dụ: `C:\Program Files\Java\jdk-17\bin`.

#### Bước 4: Kiểm tra cài đặt
- Mở Command Prompt và gõ lệnh:
  ```bash
  java -version