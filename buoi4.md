1. Hàm xử lý mảng
- count(): đếm số lượng phẩn tử trong mảng
- in_array($value,$array): kiểm tra xem có tồn tại value đó không, trả về true(1) hoặc false(0)
- array_keys($array): lấy ra các key của mảng(cho vào vòng lặp)
foreach($key as $item){
    echo $item;
}
- array_values($array): lấy ra các value
- sort ($array): sắp xếp  tăng dần
$ngoc = [4,2,5,7,8,9,0];
sort($ngoc)
foreach($ngoc as $item){
    echo $item;
}
- rsort ($array): sắp xếp giảm dần
- array_push($array,$value): thêm 1 phần tử vào cuối mảng
$mang1 = ['php','js'];
array_push($mang1,'mysql');
foreach($mang1 as $item){
    echo $item;
}
- array_pop($array): xóa 1 phần tử cuối mảng
- array_unshift($array,$value): thêm 1 phần tử vào đầu mảng
- array_shift($array): xóa 1 phần tử đầu mảng
- array_filter($array,"callback"): lọc sữ liệu theo đk cụ thể được gọi trong callback
$nbs = [1,2,3,4,5,6,54,34];
$result= array_filter($nbs, function($nb){
    return $nb % 2 == 0;
});
echo '<pre>';
print_r($result);
echo '</pre>';
- array_unique($array): lọc ra các phần tử trùng lặp
- array_merge($array1,$array2): nối 2 mảng
- explode($delimiter,$string): tách chuỗi thành mảng
- implode($delimiter,$array): gộp mảng thành chuỗi
2. Hàm xử lý chuỗi
- nối chuỗi: dùng dấm chấm(.)
- strlen(): đếm chuỗi trả về độ dài tính cả khoảng trắng
- str_word_count(): đếm xem có bao nhiêu từ không tính khoảng trắng, ko hỗ trợ tiếng việt
- strrev(): đảo ngược chuỗi
- strpos($array, 'chữ cần tìm'): tìm chuỗi con ở trong chuỗi cha
- str_replace('chữ cần sửa','chữ thay thế',$array): thay thế  
- substr($array, vị trí cắt, độ dài cần cắt): cắt chuỗi, nếu không điền vị trí độ dài cần cắt thì sẽ cắt đến hết chuỗi
- strtolower($array): chuyển toàn bộ chuỗi thành chữ in thường
- struplower($array): chuyển toàn bộ chuỗi thành chữ in hoa
- ucfirst($array): tự động viết hoa chữ đầu tiên trong chuỗi
- ucword($array): tựu động viết hoa chữ đầu tiên trong mỗi từ
- trim(): xóa khoảng trắng thừa cả khoảng trắng đầu và cuối
- ltrim(): xóa khoảng trắng trước
- rtrim(): xóa khoảng trắng sau
- strcmp(): ss 2 chuỗi, phân biệt chữ hoa và chữ thường(bảng ASCII)
- strcasecmp(): ss 2 chuỗi, không phân biệt chữ hoa hay thường
- str_pad($string, số kí tự cần đạt đến, 'kí tự cần thêm vào',)
- strip_tags(): xóa thẻ HTML
- htmlspecialchars(): chuyển kí tự HTML thành mã
3. Hàm mã hóa
- md5()
- sha1()
- base64_encode(): mã hóa base64
- base64_decode(): giải mã base64