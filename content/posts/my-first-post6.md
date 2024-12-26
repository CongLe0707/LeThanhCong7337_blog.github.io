---
date : 2024-12-26T21:18:44+07:00
draft : false
title : 'Lập trình JavaScript cơ bản'
---
# Lập trình JavaScript cơ bản

JavaScript là ngôn ngữ lập trình phổ biến được sử dụng để tạo ra các trang web động và tương tác. Để làm quen với JavaScript, bạn cần nắm vững cú pháp cơ bản. Dưới đây là những khái niệm cơ bản về cú pháp của JavaScript.

## 1. Khai báo biến

JavaScript hỗ trợ ba cách để khai báo biến:

- **`var`**: Đã lỗi thời và ít được sử dụng, nhưng vẫn tồn tại để hỗ trợ tính tương thích ngược.
- **`let`**: Được sử dụng để khai báo biến có phạm vi cục bộ trong phạm vi lặp lồng (`loop`) hoặc khối lệnh (`block`).
- **`const`**: Được sử dụng để khai báo biến có giá trị không thay đổi sau khi đã được gán.

Ví dụ:

```javascript
var name = "John";
let age = 25;
const pi = 3.14;
```
## 2. Kiểu dữ liệu
JavaScript có sáu kiểu dữ liệu cơ bản:

- **`String`** (Chuỗi): "Hello World"
- **`Number `**(Số): 42, 3.14
- **`Boolean`** (Boolean): true hoặc false
- **`Null`** (Null): null
- **`Undefined`** (Không xác định): undefined
- **`Object`** (Đối tượng): Ví dụ, { name: "John", age: 25 }
## 3. Câu lệnh điều kiện
JavaScript hỗ trợ ba loại câu lệnh điều kiện chính:

- **`if`**: Điều kiện đơn giản, thực hiện hành động nếu điều kiện đúng.
- **`else`**: Điều kiện ngược, thực hiện hành động nếu điều kiện if không đúng.
- **`else if`**: Điều kiện lồng nhau.
Ví dụ:

```javascript
if (age > 18) {
  console.log("Bạn đã trưởng thành");
} else {
  console.log("Bạn chưa trưởng thành");
}
```
## 4. Vòng lặp
JavaScript hỗ trợ ba loại vòng lặp cơ bản:

- **`for`**: Vòng lặp với điều kiện lặp rõ ràng.
- **`while`**: Vòng lặp kiểm tra điều kiện trước mỗi lần lặp.
- **`do...while`**: Vòng lặp kiểm tra điều kiện sau mỗi lần lặp.
Ví dụ:

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i);
}

let i = 0;
while (i < 10) {
  console.log(i);
  i++;
}

do {
  console.log(i);
  i++;
} while (i < 10);
```
## 5. Hàm
JavaScript hỗ trợ việc khai báo hàm theo hai cách:

- **`Hàm biểu thức`**:
 Ví dụ, 
 ```javascript
 const greet = function() { 
    console.log("Hello"); 
}
```
- **`Hàm định danh`**: 
Ví dụ, 
 ```javascript
function greet() { 
    console.log("Hello"); 
}
```
- Bạn có thể truyền tham số vào hàm và trả về giá trị:

Ví dụ, 
 ```javascript
function sum(a, b) {
  return a + b;
}
console.log(sum(2, 3)); // Output: 5
```
## 6. Đối tượng
JavaScript hỗ trợ lập trình hướng đối tượng (OOP), và bạn có thể tạo đối tượng bằng cách sử dụng {}:

 ```javascript
const person = {
  name: "John",
  age: 25,
  greet: function() {
    console.log("Hello, " + this.name);
  }
};

person.greet();
``` 
## 7. Các phương thức phổ biến
Một số phương thức phổ biến trong JavaScript:

- **`alert`**: Hiển thị hộp thoại thông báo.
- **`console.log`**: Xuất thông báo lên cửa sổ console.
- **`prompt`**: Yêu cầu người dùng nhập thông tin.
- **`confirm`**: Hiển thị hộp thoại xác nhận với hai nút OK và Cancel.
## 8. Xử lý sự kiện
JavaScript hỗ trợ xử lý sự kiện cho các yếu tố HTML:

 ```javascript
document.getElementById("btn").addEventListener("click", function() {
  console.log("Button clicked");
});
```
-   Với những khái niệm cơ bản này, bạn có thể bắt đầu xây dựng các ứng dụng web đơn giản với JavaScript. Hãy thực hành và khám phá thêm các tính năng nâng cao của JavaScript để trở thành một lập trình viên web giỏi!