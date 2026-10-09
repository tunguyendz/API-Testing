# BÁO CÁO THỰC HÀNH KIỂM THỬ API BẰNG POSTMAN
Họ và tên: Nguyen Trung Tu
Môn học: Software Testing
Công cụ: Postman
Chủ đề: Thực hành kiểm thử API
## 1. Mục tiêu

Mục tiêu của bài thực hành là tìm hiểu và sử dụng công cụ Postman để kiểm thử API. Bài thực hành giúp sinh viên nắm được quy trình gửi HTTP request, kiểm tra HTTP response, xây dựng test case và viết script kiểm thử tự động.

## 2. Môi trường kiểm thử

* Công cụ: Postman.
* API sử dụng: JSONPlaceholder.
* Base URL: `https://jsonplaceholder.typicode.com`.
* Tài nguyên kiểm thử: Posts.
* Các phương thức: GET, POST, PUT, DELETE.
* Định dạng dữ liệu: JSON.
  

## 3. Phương pháp kiểm thử

Bài thực hành sử dụng phương pháp kiểm thử hộp đen, tập trung kiểm tra đầu vào và kết quả phản hồi của API mà không cần biết chi tiết cách triển khai bên trong.

Các bước thực hiện bao gồm:

1. Xây dựng các ca kiểm thử dựa trên yêu cầu.
2. Tạo request trong Postman.
3. Gửi request và kiểm tra response.
4. Viết script tự động kiểm tra mã trạng thái, dữ liệu và thời gian phản hồi.
5. Lưu request trong Collection.
6. Chạy toàn bộ Collection và tổng hợp kết quả.

## 4. Nội dung kiểm thử

### 4.1. Kiểm thử GET

Sử dụng GET để lấy thông tin bài viết theo ID. Kiểm tra mã trạng thái HTTP, định dạng JSON, ID trả về và sự tồn tại của các trường dữ liệu cần thiết.
<img width="1826" height="624" alt="image" src="https://github.com/user-attachments/assets/76a88cba-158d-4ad6-8a0b-341c5e99835a" />


### 4.2. Kiểm thử POST

Sử dụng POST để gửi dữ liệu bài viết mới. Kiểm tra mã trạng thái phản hồi, định dạng JSON và sự chính xác của các trường title, body, userId.

### 4.3. Kiểm thử PUT

Sử dụng PUT để gửi yêu cầu cập nhật bài viết. Kiểm tra mã trạng thái và dữ liệu được phản hồi sau khi gửi yêu cầu.

### 4.4. Kiểm thử DELETE

Sử dụng DELETE để gửi yêu cầu xóa bài viết. Kiểm tra mã trạng thái và nội dung phản hồi.

### 4.5. Kiểm thử lỗi

Gửi request đến endpoint không tồn tại để kiểm tra API có trả về mã trạng thái phù hợp hay không.

## 5. Kết quả kiểm thử

Kết quả được ghi nhận từ Postman sau khi chạy từng request và toàn bộ Collection. Các test case được đánh giá dựa trên sự phù hợp giữa kết quả thực tế và kết quả mong đợi.

Bảng tổng hợp cần ghi rõ mã test case, phương thức HTTP, endpoint, kết quả mong đợi, kết quả thực tế và trạng thái Passed/Failed.

## 6. Nhận xét

Postman hỗ trợ việc kiểm thử API thông qua giao diện trực quan và khả năng viết script tự động. Việc sử dụng Collection giúp tổ chức các request khoa học, dễ quản lý và chạy lại nhiều lần.

Các test case bao gồm cả trường hợp thành công và trường hợp lỗi giúp đánh giá API ở nhiều tình huống khác nhau.

## 7. Kết luận

Qua bài thực hành, em đã tìm hiểu cách sử dụng Postman để kiểm thử các phương thức GET, POST, PUT và DELETE. Em đã thực hành kiểm tra mã trạng thái HTTP, dữ liệu JSON, xây dựng test script tự động và sử dụng Collection Runner để tổng hợp kết quả.

Bài thực hành giúp em hiểu rõ hơn về quy trình kiểm thử API và vai trò của kiểm thử tự động trong việc nâng cao chất lượng phần mềm.

**Ghi chú:** JSONPlaceholder là API mô phỏng phục vụ học tập. Các thao tác POST, PUT và DELETE không được lưu bền vững như trên một hệ thống thực tế.
