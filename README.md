# 🌾 IBM Food Trust Blockchain App

Ứng dụng Flask mô phỏng nền tảng IBM Food Trust giúp **đăng ký**, **truy xuất nguồn gốc**, **quản lý chuỗi cung ứng** và **chứng minh chất lượng nông sản** bằng công nghệ Blockchain.

> ✅ Dành cho mô phỏng giáo dục, minh họa cách truy xuất nông sản minh bạch và an toàn.
### 📦 Tính năng chính
✅ Đăng ký nông sản (ID, nông dân, chứng nhận…)

✅ Cập nhật chuỗi cung ứng (đóng gói, vận chuyển, tiêu thụ)

✅ Cảnh báo sản phẩm quá hạn (>7 ngày chưa bán)

✅ Tải file PDF chứng nhận sản phẩm

✅ Tạo mã QR truy xuất chi tiết

✅ Tìm kiếm sản phẩm theo tên hoặc ID

## 🛠️ Công nghệ sử dụng

### 🔗 Backend
- **Python 3.10+**
- **Flask** – Web Framework
- **Jinja2** – Template Engine
- **qrcode** – Tạo mã QR
- **Werkzeug** – File upload
- **Base64, io, datetime** – Xử lý ảnh và dữ liệu

### 💾 Blockchain
- Blockchain đơn giản viết bằng Python
- Dữ liệu không mất khi ghi vào file (tùy chỉnh `blockchain.py`)

---

## 📁 Cấu trúc dự án

---
ibm-food-trust/

├── app.py # Flask app chính

├── blockchain.py # Class Blockchain và Block

├── requirements.txt # Các thư viện cần thiết

│

├── templates/ # Giao diện HTML

│ ├── base.html # Layout Bootstrap

│ ├── home.html # Trang chủ

│ ├── register.html # Đăng ký sản phẩm

│ ├── products.html # Danh sách

│ └── product_detail.html # Chi tiết, upload, QR

│

├── uploads/ # Tự tạo, lưu file PDF

└── static/ # (Tuỳ chọn) CSS, JS


## 🚀 Cài đặt và chạy thử

### ⚙️ Yêu cầu hệ thống
- Python 3.10 trở lên
- pip (trình quản lý gói)
  
### 📦Bước 1: Clone dự án
git clone https://github.com/khuyennn97/ibm-food-trust.git
cd ibm-food-trust
### 📥 Bước 2: Cài thư viện
pip install -r requirements.txt
### ▶️ Bước 3: Chạy ứng dụng Flask
python app.py
Truy cập tại: http://localhost:5000
🌐 Triển khai trên Render
  1.Push code lên GitHub
  2.Truy cập https://render.com
  3.Chọn New Web Service
  4.Kết nối GitHub → chọn repo ibm-food-trust
  5.Start command:
    python app.py
  6.Build command: (Để trống hoặc dùng pip install -r requirements.txt)
