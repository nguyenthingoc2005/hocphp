1. Giới thiệu 1 số hàm built_in
- alert
- console
- confirm
- prompt
- setTimeout(function(){
    alert('Thong bao')
},1000)
- setInterval(function() {
    console.log('Đây là log')
},1000)
2. Giới thiệu về toán tử trong js
- Toán tử số học: + - *  **(lũy thừa) %(chia lấy số dư) ++(tăng 1 giá trị số) --(giảm 1 giá trị số)
- Prefix(tiền tố) & Postfix(hậu tố): toán tử ++ --
- Toán tử gán
- Toán tử so sánh: = !=(k bằng) > < <= >=
- Toán tử logic: &&(và), ||(or), !(not)
- Toán tử chuỗi(string operator): nối chuỗi bằng dấu +
- Boolean trả về true hoặc false
- If - else: if(đk){
}else{}
- 0, false, '', "", undefined, NaN, null kiểu boolean trả về false còn lại trả về false
3. Kiểu dữ liệu trong Javascrip
- Dữ liệu nguyên thủy - primitive data
+ number: console.log(typeof (biến))
+ string: console.log(typeof (biến))
+ boolean: console.log(typeof (biến))
+ undefined: console.log(typeof (biến))
+ null: console.log(typeof (biến)) -> object
+ symbol: var id = Symbol('id); unique
- Dữ liệu phức tạp - complex data
+ function
+ object: var myObject = {
    name: 'Ngoc',
    age: 18,
    address: 'Hai Duong',
    myFunction: function(){
        alert('Hi xin chao');
    }
};
var myArray = [
    'Javascript',
    'PHP',
    'Ruby'
];
4. Toán tử so sánh phần 2
- So sánh ===: tuyệt đối
- So sánh !=: khác
- So sánh !==: khác tuyệt đối
5. Chuỗi trong Javascript
- Tạo chuỗi
+ Các cách tạo chuỗi:
var fullName = "ngoc";
var fullName = new String('ngoc');
- Một số case sử dụng backslash(\): var fullName = 'ngoc la \'cong chua\'';
- Xem độ dài chuỗi: console.log(fullName.length)
- Chú ý độ dài khi viết code