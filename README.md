# Postman_API

API Testing Report – Reqres API

## 1. Giới thiệu.

- Tên dự án: Kiểm thử API bằng Posman
- Ngày thực hiện: 19/06/2025
- Người thực hiện: Nguyễn Thị Cẩm Tú
- MSV: 22010230
- Môi trường  kiểm thử: Posman
- Phương pháp kiểm thử: Kiểm thử thử công, kiểm thử tự động.

Mục tiêu:
- Gửi request đến API
- Viết script kiểm thử
- Tự động hóa kiểm thử bằng dòng lệnh
- Tạo báo cáo minh họa kết quả

---

## 2. Công cụ sử dụng

| Tên công cụ | Mục đích                         |
|-------------|----------------------------------|
| Postman     | Tạo, gửi và test API request     |
| Newman      | Chạy collection từ CLI           |
| Node.js     | Cần thiết để chạy Newman         |

## 3. API được kiểm thử.

| Method | Endpoint                       | Mô tả                        |
|--------|--------------------------------|------------------------------|
| GET    | /api/users?page=2             | Lấy danh sách người dùng     |

## 4. Kiểm thử bằng Posman.

a. Tạo, gửi và test API request:

Thêm Request:
GET: https://reqres.in/api/users?page=2
POST: https://reqres.in/api/users
PUT: https://reqres.in/api/users/2
DELETE: https://reqres.in/api/users/2
![Screenshot (1356)](https://github.com/user-attachments/assets/3e436620-604d-49fc-ba4b-2d6747e04bc7)

b. Chạy collection từ CLI:

- Xuất collection (.json file): Mở terminal, cài Newman nếu chưa có:
npm install -g newman
- Chạy kiểm thử:
newman run collection.json

![Screenshot (1364)](https://github.com/user-attachments/assets/d5885092-2748-4efe-b15b-8610102750ed)

![Screenshot (1365)](https://github.com/user-attachments/assets/a9071c9a-426a-4ef3-b487-716dfebb0ce8)

## 5. Tổng kết.

a. Kết quả kiểm thử:
Tổng số request: 1
Tổng số test: 2	
Pass: 2	
Fail: 

b. Kết luận: 
Bài kiểm thử đã thực hiện thành công việc gửi request và kiểm tra phản hồi từ API. Dựa vào script, ta đã xác định đúng mã phản hồi và cấu trúc dữ liệu trong body. Đây là tiền đề tốt cho việc tự động hóa test backend API trong các dự án thực tế.


---
