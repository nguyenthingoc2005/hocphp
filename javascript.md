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
- Template string ES6
var firstName = 'Ngoc';
var lastName = 'Nguyen';
console.log(`Tôi là: ${firsstName} ${lastName}`);
6. Làm việc với chuỗi: var myString = 'Hoc JS tai F8';
- length: console.log(myString.length); -> độ dài chuỗi
- find index: console.log(myString.indexOf('JS')) -> tìm kiếm vị trí (k có trả về -1) (lastIndexOf: vị trí cuối cùng; search: k tìm được bằng cách truyền tham số thứ 2)
- cut string: console.log(myString.slice(4,6)) -> cắt chuỗi
- replace: console.log(myString.replace('JS', 'Javascript')) -> thay thế{console.log(/JS/g, 'Javascript') -> thay thế tất cả}
- convert to upper case: console.log(myString.toUpperCase()) -> thay tất cả thành chữ in hoa
- convert to lower case: console.log(myString.toLowerCase()) -> thay tất cả thành chữ in thường
- trim: console.log(myString.trim()) -> bỏ khoảng trắng đầu cuối
- split: var languages = 'JS, PHP, Ruby';
console.log(languages.split(', )) -> lấy ra thành mảng từ 1 chuỗi
- get a charscter by index: console.log(myString.charAt(0)) -> lấy kí tự theo vị trí
7. Kiểu số trong JS
- Tạo giá trị number:
+ C1 var age = 18; var PI = 3.14; 
+ C2 var ortherNumber = new Number(9);
- Làm việc với number
+ console.log( typeof age.toString());
+ console.log(PI.toFixed());
8. Mảng trong JS
- Tạo mảng: var languages = ['JS', 'PHP', 'Ruby'];
- Kiểm tra data type: console.log(Array.isArray(languages))
8. Làm việc với Array
- to string: console.log(languages. toString()); -> chuyển sang chuỗi 
- join: console.log(languages. join(', '));
- pop: xóa phần tử cuối mảng và trả về phần tử đã xóa
- push: thêm phần tử cuối mảng và trả về độ dài mảng mới
- shift: xóa phần tử đầu mảng và trả về phần tử đã xóa
- unshift: thêm phần tử đầu mảng và trả về độ dài mảng mới
- spliicing: languages.splice(1, 2, 'Dart') -> xóa 1 element bất kì
- concat: nối array console.log(languages.concat(languages2))
- slicing: cắt 1 vài element của mảng console.log(languages.slice(1,2))