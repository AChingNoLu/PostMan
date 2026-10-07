# Thực hành Postman: Gửi yêu cầu GET và POST tới API

## 1. Giới thiệu

Postman là công cụ dùng để thiết kế, gửi và kiểm thử các yêu cầu HTTP tới API mà không cần viết mã. Trong bài thực hành này, em sử dụng Postman để:

- Gửi yêu cầu **GET** nhằm lấy dữ liệu từ một API mẫu.
- Gửi yêu cầu **POST** nhằm thêm mới dữ liệu.
- Gửi yêu cầu **GET** tới một trang web thông thường để so sánh định dạng dữ liệu trả về.

API mẫu được sử dụng: [JSONPlaceholder](https://jsonplaceholder.typicode.com/) – dịch vụ API giả lập miễn phí dùng cho mục đích học tập và kiểm thử.

## 2. Gửi yêu cầu GET (Lấy dữ liệu)

- Phương thức (Method): `GET`
- URL: `https://jsonplaceholder.typicode.com/users`

### Các bước thực hiện

1. Chọn phương thức **GET** từ danh sách thả xuống bên cạnh thanh URL.
2. Nhập chính xác đường dẫn `https://jsonplaceholder.typicode.com/users`.
3. Nhấn nút **Send** (màu xanh dương).

### Kết quả trả về (Response)

- **Status:** `200 OK` – yêu cầu được xử lý thành công.
- **Body:** danh sách người dùng ở định dạng JSON, gồm các thông tin chi tiết như `id`, `name`, `username`, `email`, `address`, ...

![Kết quả gửi yêu cầu GET tới /users](https://github.com/user-attachments/assets/0b201181-2f24-4efc-a66f-3ac43e3253e4)

*Hình 1: Gửi yêu cầu GET và nhận danh sách người dùng.*

## 3. Gửi yêu cầu POST (Thêm mới dữ liệu)

- Phương thức (Method): `POST`
- URL: `https://jsonplaceholder.typicode.com/users`

### Kết quả trả về (Response)

- **Status:** `201 Created` – tài nguyên mới đã được khởi tạo thành công.
- **Body:** trả về `id` của bản ghi vừa tạo (ví dụ: `"id": 11`).

> **Lưu ý:** JSONPlaceholder là API giả lập nên dữ liệu gửi lên không thực sự được lưu lại; server chỉ phản hồi như thể bản ghi đã được tạo.

![Kết quả gửi yêu cầu POST tới /users](https://github.com/user-attachments/assets/86d69886-11c4-4781-b34d-d5106d7681df)

*Hình 2: Gửi yêu cầu POST và nhận phản hồi 201 Created.*

## 4. Thử nghiệm với trang web khác (VnExpress)

Để kiểm tra sự khác biệt giữa API và trang web thông thường, em thay đổi URL sang trang chủ VnExpress.

- Phương thức (Method): `GET`
- URL: `https://vnexpress.net/`

### Kết quả trả về (Response)

- **Status:** `200 OK`.
- **Body:** tab hiển thị định dạng **HTML** chứa toàn bộ mã nguồn trang chủ VnExpress, thay vì dữ liệu JSON thuần túy.

![Kết quả gửi yêu cầu GET tới vnexpress.net](https://github.com/user-attachments/assets/419bbe8e-5cfd-4de7-822b-f148d9559e04)

*Hình 3: Gửi yêu cầu GET tới trang web VnExpress.*

