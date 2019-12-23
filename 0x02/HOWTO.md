Bài 2

Trong code có đoạn sử dụng hàm so sánh strcasecmp() 2 string . Nhưng nếu giá trị truyền vào là 1 mảng thì sẽ lỗi và return 0
=> Dùng postman,POST giá trị đến http://ctfq.sweetduet.info:10080/~q32/auth.php và trong mục Body add Key là 1 mảng password[] và giá trị bất kỳ ví dụ 123
khi đó kết quả trả về sẽ có Flag : FLAG_VQcTWEK7zZYzvLhX
 
Bài 1

ở cuối đoạn code file 2fa71019.php ta có thể thấy đoạn:
 eval/*nimshyqhtb*/(ugqkkci($ssyowfjkl, $cxcejhixho));

Trong đó hàm hàm eval() trong PHP chuyển một chuỗi được nhập sang PHP và thực thi nó
 Ví dụ : eval("echo \"Hello world\";"); // Output: Hello world
Khi đó ta có thể đoán được hàm ugqkkci() sẽ là là hàm decode của đoạn code thực thi chính đã bị encrypted trong biến $ssyowfjkl

Vậy bây giờ thay vì cho nó thực thi bởi eval() thì sẽ cho echo kết quả trả về từ hàm ugqkkci() và kết quả khi đi code trong file ex1_decoded



