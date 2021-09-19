# Bài tập khởi động

## Hiển thị trên trình duyệt dòng chữ **Welcome to PHP**. 
Các bước thực hiện:
- Bước 1: Tạo thư mục **BaitapPHP** nằm trong thư mục `C:\xampp\htdocs` (Nếu thư mục web_root của XAMPP trên máy bạn mặc định nằm trên ổ đĩa `C:`).
- Bước 2: Khởi động XAMPP -> Nhấn vào nút 'Start' của Module **Apache**.
- Bước 3: Mở trình soạn thảo Sublime Text (Nếu bạn sử dụng phần mềm này để soạn thảo PHP).
- Bước 4: Tạo một file mới, lưu file với tên là `welcome.php` trong thư mục **BaitapPHP**
- Bước 5: Nhập nội dung sau vào cửa sổ soạn thảo:
```php
<?php
    echo "Welcome to <b style: color = 'blue'> PHP </b>";
?>
```
- Bước 5: Nhấn *Ctrl + S* lưu lại.
- Bước 6: Mở trình duyệt web (Ví dụ: Google Chrome), trên thanh địa chỉ gõ vào: `http://localhost`.
- Bước 7: Click chọn file cần thực thi (Ví dụ: `welcome.php`) rồi xem kết quả trên trình duyệt.

**Lưu ý:**
- Nếu port mặc định không phải là 80 thì trên thanh địa chỉ bạn gõ vào theo cú pháp sau: `http://localhost:tên-port`


### Thực hiện lại các ví dụ minh họa trong Chủ đề 2. PHP cơ bản.


# Bài tập nâng cao
## Bài 1
Tạo ngẫu nhiên 1 số nguyên có giá trị trong khoảng [10,1000]. Sau đó thực hiện các yêu cầu sau:
a/ Hiển thị các số nguyên tố nhỏ hơn số nguyên được tạo.
b/ Cho biết số nguyên này có bao nhiêu chữ số.
c/ Cho biết chữ số lớn nhất trong số nguyên này.

## Bài 2
Tạo một số nguyên dương ngẫu nhiên có giá trị trong khoảng [1,10]. In ra bảng cửu chương tương ứng với giá trị đó.
Ví dụ: Nếu số nguyên được tạo ra là 3, thì xuất ra bảng cửu chương 3.

## Bài 3
In ra trình duyệt các bảng cửu chương từ 1 đến 10.

## Bài 4
Hiển thị ma trận có kích thước mxn, với m và n là 2 số nguyên dương được tạo ngẫu nhiên trong khoảng [2,5], và các phần tử trong ma trận có giá trị thuộc [-100, 100].
