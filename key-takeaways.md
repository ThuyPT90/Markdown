# Version control system
- Hệ thống quản lý các phiên bản
# Git
## Vì sao phải dùng:
- Do trong cùng dự án sẽ dùng chung Repo. Sử dụng git dễ quản lý
## Git khác với các VSC khác:
- Tính năng: Nhiều tính năng vượt trội: branchinh, tốc độ sử lý nhanh
- Chi phí: Free
- Phổ biến nhiều công ty dùng
## Khác biệt giữa Git và Github
![Khác biệt giữa Git và GitHub](https://prnt.sc/V8LQuK5fzNmX)
- Git phần mềm trên máy. GitHub là công cụ trên website. 
- GitHub để upload Git repository lên
## Git có 3 states: 
- Sinh ra 2 vùng khi tạo lệnh git init (chỉ khởi tạo 1 lần duy nhất)
1. Working directory: chứa file tạo mới hoặc file có sự thay đổi
2. Staging area: Là những file sau khi gõ lệnh add 

3. Repository: File sau khi push lên
git comit -m"<commit message>"
## Git-keytakeaways:
### 1. khởi tạo:
- git init
### 2. Cấu hình:
 *Cấu hình cho 1 máy:*
 - git config user.name "<name>". 
 - git config user.email "<email>"

*Cấu hình cho toàn bộ máy tính:*
- git config --global user.name "<name>"
- git config --global user.email "<email>"
### 3. Thêm file vào vùng Staging:
 *Đưa 1 file lên*
- git add <file_name> 

 *Đưa n file lên*
- git add <file_name1> <file_name2> ... <file_name n>

*Đưa tất cả file lên staging:* 
- git add .

**Lưu ý**
- file_name: cần đường dẫn đầy đủ. Để lấy đường dẫn có thể thao tác: trỏ và file cần đưa lên > chuột phải > copy path
#### Xem status file:
- Git status
- File màu xanh là vùng staging
- File đỏ là vùng working directory
### 4. Commit
- git commit -m"<message">
**Kiểm tra lịch sử commit"
- git log
### Commit convention: 
- <type> <short_description 50 kí tự>
- Chore: sửa nhỏ lẻ, chính tả, xóa file không dùng tới
- Feat: thêm tính năng mới
- Fix: sửa lỗi 
# Javascript basic
## Cách show dòng text "Hello World!"
1. console.log("Hello World!");
2. Chạy lệnh: Node <đường dẫn thư mục>
## Variable
1. Khai báo: 
- var <tên biến> = <giá trị>;
- let <tên biến> = <giá trị>;
- const <tên biến> = <Giá trị>
2. Lưu ý 
- Tên biến bắt đàu bằng chữ hoặc gạch chân hoặc $
- Không chứa dấu cách, không chứa từ khóa (Var, let, for, if...)
- Tên biến sẽ có phân biệt chữ hoa chữ thường
3. So sánh Var, let, const
- Var/let: khi biến sẽ gán lại được 
- Const: biến không gán lại được 
- Var: biến cục bộ. Let: biến dùng trong phạm vi {}
## Type data:
1. String: Khai báo một chuối chứa trong ""
- let name = "ThuyPT"
2. Number: khai báo số nguyên, thập phân
- let age = 18
- let num = 18.1
3. Boolean: 
- let isname = true;
## Kiểu so sánh 
1. So sánh hơn kém >, <
2. So sánh bằng: ==, ===, !=, !==, >=, <=
- ví dụ:
 let a = 5;
 let b = 3;
 let compare = a > b;
 console.log (campare);-> kết quả show là: true
## Toán tử 1 ngôi: unary opeator
- Dùng tăng giảm giá trị
 i++/ i--
- Tăng giảm 2 giá trị
i+=2/ i-=2
## conditional: điều kiện
**Cú pháp** if (<điều kiện đúng>) {
    // code sẽ chạy
}
## Loop: Vòng lặp
for (<khởi tạo>; <điều kiện dừng>; <điều kiện tăng>) {
    //code
}