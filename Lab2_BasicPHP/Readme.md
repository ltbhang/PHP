<h1>Bài tập thực hành PHP cơ bản</h1>

- [Bài tập khởi động](#bt_khoidong) <br>
- [Bài tập nâng cao](#bt_nangcao) <br>

## Bài tập khởi động <a name="bt_khoidong" />

### Hiển thị trên trình duyệt dòng chữ **Welcome to PHP**. 
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
- Bước 6: Mở trình duyệt web (Ví dụ: Google Chrome), trên thanh địa chỉ gõ vào: `http://localhost/BaitapPHP`.

**Lưu ý:** Nếu port mặc định không phải là 80 thì trên thanh địa chỉ bạn gõ vào theo cú pháp sau: `http://localhost:tên-port/Tên-thư-mục`
- Bước 7: Click chọn file cần thực thi (Ví dụ: `welcome.php`) rồi xem kết quả trên trình duyệt.

### Thực hiện lại các ví dụ minh họa trong Chủ đề 2. PHP cơ bản.


## Bài tập nâng cao<a name="bt_nangcao" />
### Bài 1
Tạo ngẫu nhiên 1 số nguyên có giá trị trong khoảng [10,1000]. Sau đó thực hiện các yêu cầu sau:

a/ Hiển thị các số nguyên tố nhỏ hơn số nguyên được tạo.

b/ Cho biết số nguyên này có bao nhiêu chữ số.

c/ Cho biết chữ số lớn nhất trong số nguyên này.

### Bài 2
Tạo một số nguyên dương ngẫu nhiên có giá trị trong khoảng [1,10]. In ra bảng cửu chương tương ứng với giá trị đó.
Ví dụ: Nếu số nguyên được tạo ra là 3, thì xuất ra bảng cửu chương 3.

*Gợi ý:*

~ Sử dụng vòng lặp để hiển thị kết quả.

### Bài 3
In ra trình duyệt các bảng cửu chương từ 1 đến 10.

*Gợi ý:*

~ Sử dụng hai vòng lặp để hiển thị kết quả.

#### Bài 4
Hiển thị ma trận có kích thước mxn, với m và n là 2 số nguyên dương được tạo ngẫu nhiên trong khoảng [2,5], và các phần tử trong ma trận có giá trị thuộc [-100, 100].

*Gợi ý:*

~ Sử dụng hai vòng lặp để tạo ma trận.
~ Sử dụng các thẻ của HTML để tạo bảng hiển thị ma trận.

### Bài 5
- Tạo ngẫu nhiên 1 số nguyên có giá trị trong khoảng [-100,100].
- Kiểm tra số nguyên này có phải là số nguyên tố. Nếu là số nguyên tố thì đưa vào lưu trữ trong tập tin có tên là *soNT.txt*.

*Gợi ý:*

~ Sử dụng các hàm thao tác trên tập tin.

~ Số nguyên tố được tìm thấy (mỗi lần thực thi chương trình) được lưu nối vào cuối file *soNT.txt*.
 
