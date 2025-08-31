1. COOKIE TRONG PHP
- Cookie là 1 tập tin nhỏ được lưu trữ trên máy người dùng (trình duyệt giúp lưu lại dữ liệu giữa các lần truy cập)
- setcookie(name, value, expire, path, domain, secure, httponly);
get cookie
+ value: giá trị của cookie
+ expire: thời điểm hết hạn (cookie chết)
+ path: đường dẫn áp dụng cookie
+ domain: tên miền mà áp dụng cookie
+ secure: true->https
+ httponly: ngăn chặn js và tăng cường bảo mật
- xóa cookie: setcookie('ngoc','2000',time() - 3600);
- setcookie('ngoc','2000',time() + 3600);
2. SESSION TRONG PHP
- Session (phiên làm việc) là nơi lưu trữ thông tin trên server cho mỗi người dùng
- Khác với cookie (lưu trên trình duyệt), session an toàn hơn vì người dùng không truy cập trực tiếp được
- session_start(); bắt buộc phải có
- $_SESION['ngoc] = 'Học lập trình PHP; tạo xong session
-if(isset($_SESSION['ngoc])){
    echo $_SESSION['ngoc];
}
- xóa session: unset($_SESSION['ngoc]);
3. Các loại lỗi trong PHP và Debug
- Parse Error: lỗi cú pháp -> PHP không chạy được
- Fatal Error: lỗi nghiêm trọng
- Warning: Cảnh báo, code vẫn chạy
- Notice: nhắc nhở nhẹ
- Exception (Exception Error): lỗi được ném ra trong khối try_catch -> có thể xử lý được
- ini_set('display_errors',1);
- ini_set('display_startup_errors',1);
- error_reporting(E_ALL): hiển thị tất cả lỗi
- try{
    đoạn code gây ra lỗi
    throw new Exception("thông báo lỗi");
}catch(Exception $e){
    xử lý khi có lỗi
    echo "Đã xảy ra lỗi:".$e -> getMessage();
}
- try{
    $age = -18;
    if($age < 0){
        throw new Exception("Tuổi không thể là số âm);
    }
    echo "Tuổi hợp lệ: ".$age;
}catch(Exception $e){
    echo "Đã xảy ra lỗi:".$e -> getMessage();
}