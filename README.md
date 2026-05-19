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

1.<img width="1592" height="1009" alt="image" src="https://github.com/user-attachments/assets/b2f9cbf1-1d0e-45b8-87f5-0fc76f888641" />
2.<img width="1612" height="1003" alt="image" src="https://github.com/user-attachments/assets/6b2cb810-2cad-4b7e-84bb-5f5686ec1e55" />
2.1.<img width="1616" height="1005" alt="image" src="https://github.com/user-attachments/assets/a75a6f4c-3537-4a6c-b3e0-ddc5316dbf4c" />
3.<img width="1604" height="992" alt="image" src="https://github.com/user-attachments/assets/53e4adab-e4b7-43c3-847f-7e8ad8fdecf8" />
3.1.<img width="1608" height="993" alt="image" src="https://github.com/user-attachments/assets/e6645602-936c-4629-b283-94068f4618cd" />
4.<img width="1596" height="995" alt="image" src="https://github.com/user-attachments/assets/cc97f1fc-1090-4cba-8bfc-a39bb06c77ea" />
4.1<img width="1603" height="992" alt="image" src="https://github.com/user-attachments/assets/0d24e036-b3db-4787-b009-6731f74403ee" />
5<img width="1611" height="997" alt="image" src="https://github.com/user-attachments/assets/3b7089da-8990-4af1-85cf-568e5f0ca0cc" />
5.1<img width="1608" height="1003" alt="image" src="https://github.com/user-attachments/assets/a7b27865-5344-4d30-bb90-0409a2e1ff23" />
6.<img width="1603" height="992" alt="image" src="https://github.com/user-attachments/assets/c7280af7-1bd6-4618-b3f3-8fd9d28d69e5" />
6.1<img width="1597" height="993" alt="image" src="https://github.com/user-attachments/assets/02b13f33-f36a-4133-910a-4289bc572033" />


