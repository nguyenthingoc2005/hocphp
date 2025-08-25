I. Tổng quan về PHP & MySQL
1. PHP là gì: nn lập trình web động
2. Ưu điểm:
- Mã nguồn mở, miễn phí
- Dễ học sễ sư dụng
- Tương thích cao
- Hiệu suất cao
- Thư viện và framework mạnh mẽ
3. Cách PHP hoạt động: hoạt động theo mô hình Client - Server
PHP thu request và xử lý trên server, từ server lấy dữ liệu từ database -> server -> response 
4. Công cụ và môi trường
II. PHP căn bản
1. Cú pháp php cơ bản
- cú pháp  <?php ?>
- file .php
- echo: in,có thể in ra nhiều tham số cách nhau bằng dấu phẩy
- print trả về giá trị 1
- cú pháp cmt: // 1 dòng, /* */nhiều dòng 
- có dấu phẩy khi kết thúc
2. Biến trong PHP
- bắt đầu bằng $
- Quy tắc đặt tên: k chứa dấu cách, phân biệt chữ hoa và chữ thường, k dùng php làm tên biến 
3. Hằng số trong php
define('SITE_NAME','ngoc');
echo SITE_NAME;

const SITE_NAME = 'ngoc';
echo SITE_NAME;
4. Kiểu dữ liệu trong PHP: 
kiểu chuỗi string
- nháy đơn '': k gọi được biến
- nháy kép "": gọi được biến
kiểu số nguyên
- var_dump(): kiểm tra giá trị của biến và in ra biến
kiểu số thực
kiểu boolean: chỉ có true hoặc flase
kiểu mảng
echo '<pre>';
print_r($arr);
echo '</pre>';
