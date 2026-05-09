# Portfolio App Hub

Website portfolio cá nhân để giới thiệu các ứng dụng, được deploy trên Vercel.

## 📁 Cấu trúc dự án

```
web/
├── index.html        # Trang chính
├── apps.js           # Danh sách ứng dụng (dữ liệu)
├── vercel.json       # Cấu hình Vercel
└── README.md         # Tài liệu này
```

## 🚀 Deploy lên Vercel

### Cách 1: Dùng Vercel CLI (Terminal)

```bash
# Cài đặt Vercel CLI (nếu chưa có)
npm install -g vercel

# Đăng nhập
vercel login

# Deploy (chạy trong thư mục dự án)
vercel

# Deploy production
vercel --prod
```

### Cách 2: Kéo thả trên Vercel.com

1. Truy cập [vercel.com](https://vercel.com) → Đăng nhập
2. Nhấn **"Add New Project"**
3. Import từ **GitHub** (đẩy code lên GitHub trước)
4. Chọn repo → Vercel tự detect là **Static Site**
5. Nhấn **Deploy** ✅

### Cách 3: Kéo thả thư mục

1. Truy cập [vercel.com/new](https://vercel.com/new)
2. Kéo thả **toàn bộ thư mục `web/`** vào trang
3. Nhấn **Deploy** ✅

## ⚙️ Cấu hình Vercel (`vercel.json`)

- **Static site** – không cần build tool
- Route `apps.js` trả về đúng `Content-Type: application/javascript`
- Mọi route khác trỏ về `index.html` (SPA support)
- Cache 1 giờ, stale-while-revalidate 24 giờ

## ✏️ Thêm/sửa ứng dụng

Chỉnh sửa file `apps.js`:

```js
const apps = [
  {
    id: 4,
    title: "Tên ứng dụng mới",
    category: "Giáo dục",          // hoặc: Giải trí, Khoa học
    description: "Mô tả ngắn gọn về ứng dụng...",
    tags: ["HTML", "JavaScript"],
    url: "https://link-den-app.com",
    image: "https://link-den-anh-preview.jpg"
  }
];
```

## 🌐 Môi trường yêu cầu

- Không cần Node.js hay build bước nào
- Chạy thuần HTML + JS (ES Modules)
- Tailwind CSS qua CDN
- Google Fonts qua CDN
