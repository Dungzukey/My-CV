# Portfolio CV - Ngô Mạnh Dũng

## 1. Tên dự án
Portfolio cá nhân và CV online của Ngô Mạnh Dũng

## 2. Mô tả dự án
Dự án này là một trang web portfolio cá nhân được xây dựng bằng HTML5 và CSS3, nhằm giới thiệu bản thân, kỹ năng, dự án tiêu biểu và thông tin liên hệ. Trang web có thiết kế hiện đại, tối giản, dễ đọc và tương thích với nhiều kích thước màn hình, từ điện thoại di động đến máy tính để bàn.

Trang web này phù hợp cho mục đích:
- Giới thiệu bản thân và hồ sơ nghề nghiệp
- Trưng bày dự án đã làm
- Hiển thị kỹ năng và công nghệ sử dụng
- Kết nối với nhà tuyển dụng hoặc khách hàng

## 3. Chức năng chính
- Hero section giới thiệu cá nhân
- Phần giới thiệu ngắn về bản thân
- Hiển thị danh sách kỹ năng kỹ thuật
- Phần dự án thành công với card layout
- Phần liên hệ và thông tin mạng xã hội
- Giao diện responsive trên mobile, tablet và desktop
- Tối ưu tương thích với trình duyệt hiện đại
- Điều hướng nhanh bằng navigation menu

## 4. Công nghệ sử dụng
- HTML5
- CSS3
- Flexbox
- CSS Grid
- Responsive Web Design
- Semantic HTML
- JavaScript (nếu tích hợp trong tương lai)
- Git & GitHub

## 5. Yêu cầu môi trường
Để chạy dự án, bạn cần:
- Một trình duyệt web: Chrome, Edge, Firefox, Safari
- Một máy tính có hệ điều hành Windows, macOS hoặc Linux
- Tùy chọn: Python 3 hoặc Node.js để chạy máy chủ tĩnh
- Tùy chọn: Docker nếu muốn triển khai theo container

## 6. Cài đặt
### 6.1. Tải xuống dự án
- Clone repository hoặc tải zip về máy tính
- Giải nén vào thư mục mong muốn

```bash
git clone <repository-url>
cd KT-A2.1
```

### 6.2. Mở thư mục dự án
Ví dụ:

```bash
C:\Users\<Tên_nguời_dùng>\Downloads\KT A2.1
```

## 7. Cấu hình
Bạn có thể chỉnh sửa các thông tin sau trong dự án:

### 7.1. Thông tin cá nhân
Mở file `index.html` và cập nhật:
- Tên
- Tiêu đề nghề nghiệp
- Mô tả giới thiệu
- Email
- GitHub
- LinkedIn

### 7.2. Ảnh đại diện
Trong `index.html`, kiểm tra đường dẫn ảnh:

```html
<img src="./assets/img/avatar.jpg" alt="Ảnh đại diện của Ngô Mạnh Dũng" />
```

Nếu muốn thay ảnh mới, hãy thay file trong thư mục:

```text
assets/img/
```

### 7.3. Màu sắc và giao diện
Mở file `assets/css/styles.css` và sửa các biến màu trong phần `:root`:

```css
:root {
  --color-primary: #f37221;
  --color-primary-dark: #13ecf3;
  --color-accent: #6fd7f1;
  --color-bg: #333d3d;
  --color-surface: #f159dc;
}
```

## 8. Hướng dẫn chạy thử

### 8.1. Windows
Cách 1: Mở trực tiếp file `index.html` trong trình duyệt.

Cách 2: Sử dụng Python (nếu đã cài đặt):

```powershell
cd "C:\Users\<Tên_nguời_dùng>\Downloads\KT A2.1"
python -m http.server 8000
```

Sau đó mở trình duyệt và vào:

```text
http://localhost:8000
```

### 8.2. macOS
Mở Terminal trong thư mục dự án:

```bash
cd /path/to/KT-A2.1
python3 -m http.server 8000
```

Sau đó truy cập:

```text
http://localhost:8000
```

### 8.3. Linux
Mở Terminal và chạy:

```bash
cd /path/to/KT-A2.1
python3 -m http.server 8000
```

Truy cập:

```text
http://localhost:8000
```

### 8.4. Docker
Nếu bạn muốn chạy bằng Docker, hãy tạo file `Dockerfile` trong thư mục gốc dự án với nội dung sau:

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Build image:

```bash
docker build -t portfolio-cv .
```

Chạy container:

```bash
docker run -d -p 8080:80 --name portfolio-cv portfolio-cv
```

Truy cập:

```text
http://localhost:8080
```

## 9. Cách triển khai nhanh
- Đối với website tĩnh, bạn có thể triển khai trên GitHub Pages, Netlify hoặc Vercel.
- Không cần backend.
- Chỉ cần upload toàn bộ thư mục dự án lên hosting hỗ trợ static site.

## 10. Cấu trúc thư mục
```text
KT-A2.1/
├── index.html
├── README.md
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── img/
│   │   ├── avatar.jpg
│   │   └── ...
└── ...
```

## 11. Kiểm tra và bảo trì
- Nên kiểm tra lại đường dẫn ảnh sau khi thay đổi tên file
- Đảm bảo CSS không bị lỗi khi chỉnh sửa biến màu
- Nên kiểm tra trên nhiều kích thước màn hình để đảm bảo giao diện responsive
- Nếu cần cập nhật dự án, nên giữ cấu trúc HTML sematic và rõ ràng

## 12. Thông tin liên hệ
- Họ tên: Ngô Mạnh Dũng
- Email: khaikhongsao@gmail.com
- GitHub: github.com/Ngô Mạnh Dũng
- LinkedIn: https://vi.duolingo.com

## 13. Ghi chú
Dự án này là một mẫu portfolio cá nhân đơn giản nhưng có tính ứng dụng cao, dễ tùy biến và phù hợp để làm CV online hoặc hồ sơ cá nhân trên internet.

---

© 2026 - Portfolio CV - Ngô Mạnh Dũng
