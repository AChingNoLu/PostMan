# PostMan

1. Gửi yêu cầu GET (Lấy dữ liệu)

Hình ảnh đầu tiên minh họa cách gọi phương thức GET để lấy toàn bộ danh sách người dùng từ API mẫu.

Phương thức (Method): GET

URL: https://jsonplaceholder.typicode.com/users

Cách thực hiện:

Chọn phương thức GET từ danh sách thả xuống bên cạnh thanh URL.

Nhập chính xác đường dẫn https://jsonplaceholder.typicode.com/users.

Nhấn nút Send màu xanh dương.

Kết quả trả về (Response):

Status: 200 OK (Thành công).

Body: Hiển thị danh sách dữ liệu dạng JSON chứa thông tin chi tiết của người dùng (như id, name, username, email, address,...).
<img width="1452" height="895" alt="image" src="https://github.com/user-attachments/assets/0b201181-2f24-4efc-a66f-3ac43e3253e4" />


2. Gửi yêu cầu POST (Thêm mới dữ liệu)

Hình ảnh thứ hai minh họa kết quả khi gửi yêu cầu POST lên cùng hệ thống API.

Phương thức (Method): POST

URL: https://jsonplaceholder.typicode.com/users

Kết quả trả về (Response):

Status: 201 Created (Đã khởi tạo thành công tài nguyên mới).

Body: Trả về ID của bản ghi vừa được tạo (ví dụ: "id": 11).
<img width="1901" height="1001" alt="00d20989-725e-46e2-85e4-56edd6aeddc5" src="https://github.com/user-attachments/assets/86d69886-11c4-4781-b34d-d5106d7681df" />


3. Thử nghiệm với trang web khác (Ví dụ: VnExpress)
   <img width="1900" height="1007" alt="1c750055-7ff7-4d0e-9c9f-4ef2c9b7620a" src="https://github.com/user-attachments/assets/419bbe8e-5cfd-4de7-822b-f148d9559e04" />


Hình ảnh thứ ba minh họa việc thay đổi URL để kiểm tra một trang web thông thường.

Phương thức (Method): GET

URL: https://vnexpress.net/

Kết quả trả về (Response):

Status: 200 OK.

Body: Tab hiển thị định dạng HTML chứa toàn bộ mã nguồn của trang chủ VnExpress thay vì dữ liệu JSON thuần túy.

Mẹo: Bạn có thể lưu lại các request thường dùng bằng cách bấm vào nút Save ở góc trên bên phải giao diện Postman.
