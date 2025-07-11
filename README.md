# 🌾 IBM Food Trust Blockchain App - Mô phỏng truy xuất nông sản minh bạch và an toàn.

Ứng dụng Flask mô phỏng nền tảng IBM Food Trust giúp **đăng ký**, **truy xuất nguồn gốc**, **quản lý chuỗi cung ứng** và **chứng minh chất lượng nông sản** bằng công nghệ Blockchain.

### 📦 Tính năng chính
- Đăng ký nông sản (ID, nông dân, chứng nhận…)

- Cập nhật chuỗi cung ứng (đóng gói, vận chuyển, tiêu thụ)

- Cảnh báo sản phẩm quá hạn (>7 ngày chưa bán)

- Tải file PDF chứng nhận sản phẩm

- Tạo mã QR truy xuất chi tiết

- Tìm kiếm sản phẩm theo tên hoặc ID

## 🛠️ Công nghệ sử dụng

### Backend
- Python 3.10+
- Flask – Web Framework
- Jinja2 – Template Engine
- qrcode – Tạo mã QR
- Werkzeug – File upload
- Base64, io, datetime – Xử lý ảnh và dữ liệu

### Blockchain
- Solidity - Ngôn ngữ smart contract
- Python

---

## 📁 Cấu trúc dự án


```
ibm-food-trust/
├── app.py                  # Flask application chính
├── blockchain.py          # Logic blockchain lưu trữ sản phẩm
├── requirements.txt       # Danh sách thư viện cần cài đặt
├── uploads/               # Thư mục lưu file PDF tải lên (tự tạo khi chạy)
├── templates/             # HTML templates dùng Jinja2
│   ├── base.html          # Template layout chung
│   ├── home.html          # Trang chính
│   ├── register.html      # Form đăng ký sản phẩm
│   ├── products.html      # Danh sách sản phẩm
│   └── product_detail.html # Chi tiết sản phẩm (có QR code + tải lên file)
└── static/                # (Tùy chọn) chứa CSS, JS, hình ảnh nếu dùng thêm
```

## 🚀 Cài đặt và chạy thử

### ⚙️ Yêu cầu hệ thống
- Python 3.10 trở lên
- pip (trình quản lý gói)
  
### Bước 1: Clone repository

```bash
git clone https://github.com/khuyenmn97/ibm-food-trust.git
cd ibm-food-trust
```

---

### Bước 2: Cài thư viện

```bash
pip install -r requirements.txt
```

---

### Bước 3: Chạy ứng dụng Flask

```bash
python app.py
```

Truy cập tại: http://localhost:5000

---

## 🌐Triển khai trên Render 

  1.Push code lên GitHub
  
  2.Truy cập https://render.com
  
  3.Chọn New Web Service
  
  4.Kết nối GitHub → chọn repo ibm-food-trust
  
  5.Start command:
  
    python app.py
  6.Build command: (Để trống hoặc dùng pip install -r requirements.txt)
