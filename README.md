# Tài Liệu API Quản Lý Sản Phẩm (ProductAPI_JPA)

**Base URL:** `http://localhost:8080`

| Endpoint | Method | Mô tả | Request body mẫu | Response body mẫu (thành công) | Status codes |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `/products` | **GET** | Lấy danh sách tất cả sản phẩm | Không có | `[{"id": 1, "name": "Laptop", "price": 15000.0}]` | `200` |
| `/products/{id}` | **GET** | Lấy chi tiết sản phẩm theo ID | Không có | `{"id": 1, "name": "Laptop", "price": 15000.0}` | `200`, `404` |
| `/products` | **POST** | Tạo mới một sản phẩm | `{"name": "Chuột máy tính", "price": 500.0}` | `{"id": 2, "name": "Chuột máy tính", "price": 500.0}` | `201`, `400` |
| `/products/{id}` | **PUT** | Cập nhật toàn bộ thông tin sản phẩm (phải có cả name, price) | `{"name": "Laptop Gaming", "price": 20000.0}` | `{"id": 1, "name": "Laptop Gaming", "price": 20000.0}` | `200`, `400`, `404` |
| `/products/{id}` | **PATCH** | Cập nhật một phần thông tin sản phẩm (chỉ gửi trường cần sửa) | `{"price": 18000.0}` | `{"id": 1, "name": "Laptop Gaming", "price": 18000.0}` | `200`, `404` |
| `/products/{id}` | **DELETE** | Xóa sản phẩm khỏi cơ sở dữ liệu | Không có | *(Trống)* | `204`, `404` |