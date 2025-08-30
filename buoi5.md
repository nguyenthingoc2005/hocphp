1. Phương thức GET
- GET là 1 phương thức gửi dữ liệu từ client lên server, thông qua URL
- Ưu điểm: dễ chia sẻ, dễ bug, phù hợp với tìm kiếm, lọc dữ liệu
- Nhược điêm: không bảo mật, bị giới hạn kí tự
2. Phương thức POST
- Là phương thức gửi dữ liệu từ client đến server thông qua http, không hiển thị trên URL
- Ưu điểm: dữ liệu ẩn trong request, bảo mật tốt hơn, không giới hạn ký tự (gửi nhiều dữ liệu tùy server)
- Nhược điểm: không thể kiểm tra nhanh bằng URL
3. Đệ quy trong php
- Tính giai thừa n!
function giaithua($n){
    //đk dừng
    if($n == 0){
        return 1;
    }
    return $n * giaithua($n-1)
}
echo giaithua(5);
- $_REQUEST trong php $_POST VÀ $_GET
- siêu toàn cục: $_POST VÀ $_GET, $COOKIE
- Biến toàn cục $_SERVER
4. VALIDATE: Xử lý dữ liệu nhập vào từ Form
- Tránh sai định dạng
- Ngăn chặn tấn công(XSS, SQL Ijnection)
- Đảm bảo dữ liệu sạch trước khi lưu và CSDL
=> người dùng nhập dữ liệu -> php nhập dữ liệu (POST, GET) -> Validate dữ liệu -> Hiển thị lỗi nếu có hoặc tiếp tục xử lý
5. DATE_TIME trong php
- date('Y:m:d H:i:s')
Y: năm đầy đủ(2025)
y: năm viết tắt(25)
m: tháng
d: ngày
H: giờ
i: phút
s: giây
- date_default_timezone_set('Asia/Ho_Chi_Minh');: thời gian của khu vực
- time(): thời gian timestamp (số giây từ ngày 1/1/1970 đến nay)
- strtotime()
6. UPLOAD FILE trong php
input type=file
$FILE
- phải gửi bằng phương thức POST và có enctype=multipart/form-data





