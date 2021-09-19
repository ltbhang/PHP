<h1 style="text-align:center"> Lab 1:  Cài đặt Web server </h1>

- [GIỚI THIỆU WEB SERVER](#intro) <br>
- [GIỚI THIỆU XAMPP](#intro_xampp) <br>
- [CÀI ĐẶT XAMPP](#install_xampp) <br>
- [SỬ DỤNG  VÀ QUẢN TRỊ XAMPP](#using_xampp) <br>
- [ĐỔI PORT CHO XAMPP](#change_port) <br>
- [THAY ĐỔI THƯ MỤC WEB ROOT APACHE- HTDOCS WWW](#change_root_folder) <br>


## GIỚI THIỆU WEB SERVER <a name="intro" />
•	Web Server (máy phục vụ Web): là máy tính mà trên đó cài đặt phần mềm phục vụ web, đôi khi người ta cũng gọi chính phần mềm đó là web server.

•	Tất cả các Web Server đều hiểu và chạy được các file *.htm và *.html, tuy nhiên mỗi Web Server lại phục vụ một số kiểu file chuyên biệt, ví dụ, IIS của Microsoft dành cho *.asp, *.aspx…; Sun Java System Web Server của SUN dành cho *.jsp…; Apache dành cho *.php…Tuỳ thuộc vào ngôn ngữ lập trình web mà ta lựa chọn Web Server cho phù hợp, ví dụ nếu bạn chạy PHP thì dùng Apache. 

•	Một Web Server để có thể chạy được các ứng dụng của PHP thì thường có những thành phần sau: Apache, PHP  và MySQL. Trước đây chúng ta thường phải cài từng phần riêng biệt nhưng hiện nay đã có các gói Web Server tích hợp đầy đủ các thành phần cơ bản này. 

•	Một số gói Web Server có sẵn có thể chạy được ứng dụng PHP là: AppServ, WAMP, XAMPP, Vertrigo. Các bạn chọn một trong các gói này để cài đặt Web Server là có thể chạy được ứng dụng PHP.

•   Khóa học này sử dụng XAMPP để thực hiện các bài tập minh họa.

## GIỚI THIỆU XAMPP <a name="intro_xampp"/>

•	XAMPP là chương trình tích hợp sẵn các ứng dụng cần thiết để tạo và vận hành một máy chủ web. Chữ X trong cụm từ XAMPP ám chỉ cross-platform có nghĩa là XAMPP có thể chạy trên nhiều nền tảng khác nhau như Windows, Linux, Mac, Solaris. Các ký tự còn lại trong cụm từ có ý nghĩa như sau:

- A = Apache: XAMPP bao gồm một Apache HTTP Server dùng để chạy các ứng dụng web.

- M = MySQL: XAMPP cũng bao gồm hệ quản trị cơ sở dữ liệu MySQL.

- P = PHP: ngôn ngữ lập trình PHP.

- P = Perl: ngôn ngữ lập trình Perl.

Ngoài ra, XAMPP còn có các thành phần khác như:

- PEAR (PHP Extension and Application Repository), một thư viện mã của PHP.
- phpMyAdmin: một giao diện Web-based đến MySQL server. 
- Mail server (để gửi email).


## CÀI ĐẶT XAMPP <a name="install_xampp" />

	Bước 1. Tải XAMPP về máy tính tại: https://www.apachefriends.org/download.html. 

Sau khi download thành công, double click vào file *exe* để cài đặt. 

<img src="figs/php_install_1.png"/>

	Bước 2. Click nút *Next*.

	Bước 3. Lựa chọn các service kèm theo gói XAMPP, bạn có thể tick hết vào lựa chọn để được cài đặt đầy đủ => Click nút *Next*.

<img src="figs/php_install_2.png"/>

	Bước 4: Chọn thư mục cài đặt

Theo mặc định XAMPP được cài vào đường dẫn `C:/xampp` tuy nhiên bạn có thể thay đổi đường dẫn khác. Chú ý: bạn nên thay đổi đường dẫn (ví dụ `D:/xampp`) vì nếu máy tính bạn có hư, việc ghost hay cài lại máy tính thì các ứng dụng PHP chứa trong `D:/xampp/htdocs` vẫn được bảo toàn không bị mất. Tất nhiên đây là trường hợp xấu bạn nên tránh.

<img src="figs/php_install_3.png"/>

	Bước 5. Click nút *Next* và chờ đợi trong khi XAMPP cài đặt.

<img src="figs/php_install_4.png"/>

	Bước 6. Quá trình cài đặt XAMPP hoàn tất, bạn nhấn vào nút *Finish* để kết thúc.

<img src="figs/php_install_5.png"/>

## SỬ DỤNG  VÀ QUẢN TRỊ XAMPP <a name="using_xampp" />

	Sau khi cài đặt xong, dưới khay hệ thống (Systems tray, góc dưới phía bên phải của Windows) sẽ có biếu tượng của XAMPP, bạn click vào biểu tượng đó thì cửa sổ **XAMPP Control Panel** sẽ được hiển thị. Hoặc có thể khởi động **XAMPP Control Panel** bằng cách chạy file *xampp-control.exe* trong thư mục cài đặt XAMPP.

<img src="figs/php_install_6.png"/>

	**XAMPP Control Panel**: cho phép bạn thực hiện nhiều module riêng biệt:
+ **Config**: cho phép bạn định cấu hình XAMPP cũng như các thành phần riêng lẻ.
+ **Netstat**: hiển thị tất cả các tiến trình đang chạy trên máy tính cục bộ.
+ **Shell**: mở một trình bao UNIX.
+ **Explorer**: mở thư mục XAMPP trong Windows Explorer.
+ **Services**: hiển thị tất cả các dịch vụ hiện đang chạy trong nền.
+ **Help**: cung cấp liên kết đến diễn đàn người dùng.
+ **Quit**: đóng Bảng điều khiển XAMPP.

	Click vào nút *Start* tương ứng với hai dịch vụ Apache và MySQL để khởi động hai dịch vụ này. 
Hình dưới đây thể hiện tình trạng của hai dịch vụ Apache và MySQL đều hoạt động tốt.

<img src="figs/php_install_7.png"/>

	Click vào nút *Admin* trong hàng tương ứng với dịch vụ Apache, màn hình quản trị Apache được hiển thị:

<img src="figs/php_install_8.png"/>

	Để chạy các ứng dụng PHP trong XAMPP, bạn hãy copy các dự án vào thư mục `htdocs` trong thư mục cài đặt XAMPP. Từ trình duyệt, bạn truy cập vào ứng dụng theo cấu trúc: `localhost/ten_ung_dung/ten_file`. Ví dụ ứng dụng có tên *QLbanhang* và file php là *welcome.php* thì đường dẫn sẽ là `http://localhost/QLbanhang/welcome.php`.
**Chú ý**:
	Để vào được XAMPP chúng ta có thể gõ lên trình duyệt nội dung là: http://localhost/
	Để đóng bảng điều khiển của XAMPP, bạn click vào nút *Close*. XAMPP sẽ tạm thời ẩn xuống khay hệ thống (System tray) của Windows.
	Khi cần mở bảng điểu khiển chúng ta chỉ cần click vào biểu tượng XAMPP  ở khay hệ thống của Windows.
	Để thoát khỏi XAMPP đầu tiên chúng ta click nút *Stop* ở bên cạnh Apache và MySQL sau đó click nút *Exit*.


## ĐỔI PORT CHO XAMPP <a name="change_port" />

Việc bị trùng port khi dùng XAMPP cũng là một trong những lỗi phổ biến nhất và thường gây khó khăn nhất cho bạn nào khi mới sử dụng.
### NGUYÊN NHÂN GÂY LỖI

Một nguyên nhân phổ biến của lỗi kết nối với Apache là các cổng bị chặn. Mặc định, XAMPP sẽ chỉ định máy chủ web cho cổng chính 80 và cổng SSL 443. Tuy nhiên port 80 rất phổ biến, nên nếu máy bạn có cài IIS hoặc web server nào khác thì chắc chắn sẽ bị lỗi, còn cổng SSL thường bị các chương trình khác chặn. Do đó xác suất gặp lỗi port 443 cũng khá cao.

<img src="figs/php_install_9.png"/>

Trong hình ví dụ trên, có thể cổng Tomcat đang bị chặn, nghĩa là không thể khởi động máy chủ web. Do đó, cách giải quyết thường được dùng là ta tiến hành đổi port cho XAMPP.

Ghi chú: Để biết XAMPP sử dụng port nào cho service tương ứng, tại cửa sổ **XAMPP Control Panel** bạn click vào nút *Config* -> *Service and Port settings* để biết chi tiết.

### CÁCH ĐỔI PORT
	Bước 1: Tại cửa sổ XAMPP Control Panel, click nút *Config*.

<img src="figs/php_install_10.png"/>

	Bước 2: Click nút *Service and Port Settings* như hình dưới đây.

<img src="figs/php_install_11.png"/>

	Bước 3: Tại đây bạn đổi port mặc định của Apache, ví dụ, Main port 80 thành 7070 và SSL Port 443 thành 600 -> Nhấn nút *Save*.

Bạn có thể đổi port bao nhiêu tùy thích nhưng trước khi đổi cần kiểm tra port đó đã bị sử dụng hay chưa bằng cách click vào nút *NetStat* trong **XAMPP Control Panel** để xem.

<img src="figs/php_install_12.png"/>

	Bước 4: Đổi port MySQL và các port khác nếu bị lỗi. ***Thông thường nếu mới lập trình, bạn chỉ cần đổi port của Apache là đủ***.

	Bước 5: Các bước trên chỉ mới cấu hình trên giao diện XAMPP. Bạn cần phải cấu hình trong 2 file `httpd.conf` và `httpd-ssl.conf` thì mới hoàn tất như hình sau:

<img src="figs/php_install_13.png"/>


#### Cấu hình cho `httpd.conf`: 
•	Click vào nút *Config* của dịch vụ Apache -> Click chọn `httpd.conf`, một cửa sổ Notepad sẽ hiện ra:

<img src="figs/php_install_14.png"/>

•	Tại đây, nhấn tổ hợp phím *Ctrl + F* để hiện hộp thoại tìm kiếm:

<img src="figs/php_install_15.png"/>

•	Tại đây, nhập port 80 và click Find Next để tìm và đổi số 80 thành số port (ví dụ 7070) mà bạn cấu hình như ở các bước trên.

•   Nhấn tổ hợp phím *Ctrl + S* để lưu lại các thay đổi trên file này.

#### Cấu hình cho `httpd-ssl.conf`:  thực hiện tương tự như trên, với giá trị tìm kiếm là 443 và giá trị thay thế là 600 (nếu ở bước đổi port bạn sử dụng giá trị này cho SSL port).


## THAY ĐỔI THƯ MỤC WEB ROOT APACHE- HTDOCS WWW <a name="change_root_folder" />

•	Thư mục gốc (Web root) dùng để chứa các trang web mặc định của XAMPP là `C:\xampp\htdocs` (nếu XAMPP được cài đặt ở ổ đĩa `C:`). Tất cả các website hoặc thư mục chứa website đều phải được đặt vào thư mục web root (htdocs) thì mới hoạt động được.
•	Nếu muốn bạn có thể thay đổi thư mục Web root, bạn nên tạo một thư mục web root khác nằm ở bên ngoài thư mục XAMPP để dễ sử dụng. 
•	**Các bước thực hiện**:

Ví dụ: web root của XAMPP là `c:/xampp/htdocs`.

	Bước 1. Mở file `C:\xampp\apache\conf\httpd.conf` trong Notepad

<img src="figs/php_install_16.png"/>

	Bước 2. Tìm từ *DocumentRoot* ở dòng 191:
DocumentRoot "C:/xampp/htdocs"

	Bước 3. Đổi path đến thư mục khác bạn muốn lưu dữ liệu web sử dụng về sau này cho XAMPP (Ví dụ: *D:/My Data/xampp_htdocs*)

	Bước 4. Tiếp tục, tìm dòng: <Directory "C:/xampp/htdocs"> (ở dòng 221). Đổi đường dẫn giống như Bước 3.

	Bước 5. Lưu file và khởi động lại XAMPP. 
