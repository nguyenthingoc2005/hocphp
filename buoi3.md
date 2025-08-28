1. Hàm trong php
function getStart(){

}(hàm k có tham số)
getStart();
function getStart($a,$b){

}(hàm có tham số)
getStart(2,5);
function calculator($a,$b){
    $ketqua= $a * $b;
    return $ketqua;
}
$bien_luu_ket_qua = calculator(3,4);
echo $bien_luu_ket_qua;
- Tham trị mặc định giá trọ ban đầu của tham số truyền vào
- Tham chiếu:
function calculator(&$a,&$b){
    $a += 10;
    $b += 5;
}
$a = 3;
$b = 4;
calculator($a, $b);
echo $a;
- Hàm ẩn danh
$ngoc = function($title){
    return $title;
};
echo $ngoc('hoc php');
2. Biến toàn cục và biến cục bộ
-Biến toàn cục: dùng toàn bộ chương trình, khai báo bên ngoài và sử dụng ở bất kỳ đâu
$name = 'ngoc';
echo $name;
- Biến cục bộ: dùng trong 1 hàm hoặc 1 khối lệnh cụ thể
- Biến static: 
function getAll(){
    static $a = 10;
    $a++;
    echo $a;
}
getAll();
getAll();
3. Hàm isset() và empty()
- Hàm isset() để kiểm tra xem 1 biến có tồn tại hay không. Trả về kết quả là true hoặc false
$a = 20;
var_dump(isset($a));
- Hàm empty() kiểm tra xem 1 biến có rỗng hay không.  Trả về true nếu biến rỗng, trả về flase nếu biến có giá trị
4. Câu lệnh INCLUDE, INCLUDE_ONCE(nhúng 1 lần duy nhất), REQUIRE, REQUIRE_ONCE: nhúng file
include, include_once: gặp lỗi -> tiếp tục chạy
require, require_once: gặp lỗi -> dừng chương trình
5. Mảng
- Mảng chỉ mục: bắt đầu bằng số 0
$car = array('Toyota', 'KIA','Huyndai')-khai báo cũ
$car = ['Toyota', 'KIA','Huyndai'];-khai báo mới
Toyota: key->0; value:Toyota
foreach ($car as $key => $value){
    echo $item;
    echo "<br>";
}
- Mảng kết hợp: key sẽ là chuỗi
$car = [
    'toyota' => 'camry,vios',
    'kia' => 'morning, seltos',
    'huyndai' => 'i10',
]
echo $car['kia];
foreach ($car as $key => $value){
    echo $value;
}
- Mảng đa chiều
$brand = ['toyota' => ['camry','vios','veloz'],
          'KIA' => ['morning','seltos'],
          'Huyndai' => ['i10','sentafe']
];
echo $brand['toyota'][1];
foreach ($brand as $key => $value){
    echo "Hãng xe $key gồm:";
    foreach($value as $item){
        echo $item, " ";
    }
    echo '<br>';
}


