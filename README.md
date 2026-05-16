# 🕐 Duy Minh Store - Website Bán Đồng Hồ

> **Nền tảng thương mại điện tử chuyên biệt xây dựng bằng WordPress + PHP với tích hợp Chatbot AI thông minh**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![WordPress](https://img.shields.io/badge/WordPress-5.9+-blue.svg)](https://wordpress.org/)
[![PHP](https://img.shields.io/badge/PHP-7.4+-purple.svg)](https://www.php.net/)
[![Status](https://img.shields.io/badge/status-Active-brightgreen.svg)](#)

---

## 📸 Tổng Quan

Website bán đồng hồ được phát triển bằng **WordPress CMS** kết hợp **lập trình PHP** tùy chỉnh. Dự án này được thực hiện như một bài tập chuyên đề học phần **"Phần mềm mã nguồn mở"** tại **Đại Học Điện Lực**.

Hệ thống cung cấp trải nghiệm mua sắm **đơn giản, trực quan và hiệu quả** với đầy đủ chức năng cơ bản của một nền tảng thương mại điện tử hiện đại.

### ✨ Điểm Nổi Bật

- 🔍 **Tìm kiếm & Lọc Thông Minh** - Lọc theo hãng, loại, khoảng giá, từ khóa
- 🤖 **Chatbot AI "Duy Minh AI"** - Hỗ trợ khách hàng với AI thông minh
- 🛒 **Giỏ Hàng Hiệu Quả** - Thêm/xóa/cập nhật sản phẩm dễ dàng
- 💳 **Thanh Toán Tiện Lợi** - Form checkout đơn giản, không cần đăng ký
- 📧 **Xác Nhận Email Tự Động** - Gửi chi tiết đơn hàng tới khách hàng
- 📱 **Responsive Design** - Hiển thị hoàn hảo trên mọi thiết bị
- 📰 **Blog/Tin Tức** - Giới thiệu sản phẩm và kiến thức về đồng hồ

---

## 👥 Thông Tin Dự Án

| Thông Tin | Chi Tiết |
|-----------|----------|
| **Tên Dự Án** | Website Bán Đồng Hồ - Duy Minh Store |
| **Sinh Viên Thực Hiện** | Đinh Quang Duy (23810310077)<br/>Trần Quang Minh (23810310149) |
| **Giảng Viên Hướng Dẫn** | ThS. Cấn Đức Điệp |
| **Trường** | Đại Học Điện Lực |
| **Khoa** | Công Nghệ Thông Tin |
| **Lớp** | D18CNPM1 |
| **Khóa** | 2023-2028 |
| **Học Phần** | Phần Mềm Mã Nguồn Mở |
| **Ngày Hoàn Thành** | Tháng 5 năm 2026 |

---

## 🛠️ Công Nghệ Sử Dụng

### Backend
- **CMS:** WordPress (mã nguồn mở)
- **Ngôn Ngữ:** PHP 7.4+
- **Database:** MySQL 5.7+
- **Custom:** Advanced Custom Fields (ACF), Custom Post Types

### Frontend
- **Template Engine:** PHP
- **Builder:** Elementor (Drag-Drop Page Builder)
- **CSS Framework:** Bootstrap + Custom CSS
- **Responsive:** Mobile-first approach

### Plugin & Extension
| Plugin | Mục Đích |
|--------|----------|
| **WooCommerce** | Quản lý sản phẩm & giỏ hàng |
| **Advanced Custom Fields (ACF)** | Tạo custom fields cho sản phẩm |
| **Custom Post Type UI** | Tạo custom post types (products, orders) |
| **Elementor** | Thiết kế trang web drag-drop |
| **WP Mail SMTP** | Gửi email xác nhận đơn hàng |
| **Akismet Anti-spam** | Bảo vệ bình luận spam |
| **Vietnam Checkout for WooCommerce** | Tối ưu thanh toán cho VN |

### Tools & Services
- **Quản Lý DB:** phpMyAdmin
- **Server Local:** XAMPP / LocalWP
- **Version Control:** Git
- **Repository:** GitHub

---

## 📂 Cấu Trúc Dự Án

```
Duy-Minh-Store/
├── themes/
│   └── duy-minh-theme/           # Custom WordPress Theme
│       ├── functions.php          # Hook & filter custom
│       ├── style.css              # Main stylesheet
│       ├── template-parts/        # Partial templates
│       └── assets/
│           ├── css/
│           ├── js/
│           └── images/
├── plugins/
│   └── watch-shop-custom/         # Custom Plugin
│       ├── plugin.php             # Plugin entry point
│       ├── includes/
│       │   ├── post-types.php     # Custom post types
│       │   ├── meta-boxes.php     # Custom fields
│       │   └── ajax-handlers.php  # AJAX endpoints
│       └── assets/
├── custom-code/
│   ├── chatbot-ai.php            # Duy Minh AI Chatbot
│   ├── product-filters.php       # Chức năng lọc sản phẩm
│   ├── cart-handler.php          # Xử lý giỏ hàng
│   └── enqueue.php               # Load CSS/JS
├── database/
│   └── watch-shop-backup.sql     # Database backup
├── README.md                      # File này
├── INSTALLATION.md                # Hướng dẫn cài đặt
└── .gitignore                    # Git ignore rules
```

---

## 🚀 Quick Start

### Yêu Cầu Hệ Thống
- **PHP:** 7.4 trở lên (khuyến nghị 8.0+)
- **MySQL:** 5.7 trở lên
- **WordPress:** 5.9 trở lên
- **Server:** Apache hoặc Nginx
- **Dung lượng:** Tối thiểu 2GB

### Bước 1: Chuẩn Bị

**Giả sử bạn đã cài WordPress tại:** `C:\xampp\htdocs\`

```bash
# Clone dự án hoặc download ZIP
git clone https://github.com/mingdz217/Duy-Minh-Store.git
cd Duy-Minh-Store
```

### Bước 2: Copy Files Vào WordPress

```bash
# Copy custom theme
cp -r themes/duy-minh-theme C:\xampp\htdocs\wp-content\themes\

# Copy custom plugins
cp -r plugins/watch-shop-custom C:\xampp\htdocs\wp-content\plugins\

# Copy custom code files (nếu có)
cp -r custom-code/* C:\xampp\htdocs\wp-content\plugins\watch-shop-custom\includes\
```

### Bước 3: Kích Hoạt Trong WordPress

1. Truy cập: `http://localhost/wp-admin`
2. Vào **Appearance → Themes** → Kích hoạt **Duy Minh Theme**
3. Vào **Plugins** → Kích hoạt **Watch Shop Custom Plugin**
4. Vào **ACF Fields** → Cấu hình fields tùy chỉnh

### Bước 4: Import Database (Tùy Chọn)

```bash
# Nếu muốn import dữ liệu mẫu
mysql -u root -p wordpress_db < database/watch-shop-backup.sql

# Hoặc qua phpMyAdmin:
# 1. Truy cập: http://localhost/phpmyadmin
# 2. Chọn database → Tab Import
# 3. Chọn file watch-shop-backup.sql → Execute
```

### Bước 5: Xem Website

- **Frontend:** http://localhost
- **Admin Panel:** http://localhost/wp-admin
- **phpMyAdmin:** http://localhost/phpmyadmin

---


---

## 🎯 Các Chức Năng Chính

### 1️⃣ **Danh Sách & Tìm Kiếm Sản Phẩm**
```php
// Tìm kiếm theo từ khóa, danh mục, giá
GET /shop?category=casio&price_max=5000000&search=nam
```

### 2️⃣ **Chi Tiết Sản Phẩm**
- Hiển thị thông số kỹ thuật
- Hình ảnh gallery
- Giá gốc & giá khuyến mãi
- Nút thêm vào giỏ hàng

### 3️⃣ **Giỏ Hàng & Thanh Toán**
- Quản lý giỏ hàng qua Session
- Form checkout đơn giản
- Tính toán tổng tiền tự động
- Gửi xác nhận email

### 4️⃣ **Chatbot AI "Duy Minh AI"**
```
Chatbot có khả năng:
- Nhận diện giới tính → Gợi ý sản phẩm phù hợp
- Lọc theo ngân sách → "Tìm kiếm dưới 2 triệu"
- Truy xuất thông số kỹ thuật → "Đồng hồ Casio kháng nước bao nhiêu?"
- Hướng dẫn mua hàng → Link đến checkout
```

### 5️⃣ **Quản Trị Sản Phẩm**
- Thêm/sửa/xóa sản phẩm
- Quản lý danh mục (Casio, Rolex, v.v.)
- Cập nhật tồn kho
- Xem thống kê bán hàng

---

## 📊 Công Nghệ & Kiến Trúc

### Database Schema

**Bảng Chính:**
- `wp_posts` - Sản phẩm (custom post type: product)
- `wp_postmeta` - Metadata sản phẩm (giá, hãng, loại)
- `wp_terms` - Danh mục (Casio, Rolex, Nam, Nữ)
- `wp_users` - Người dùng (admin)
- `wp_comments` - Đánh giá sản phẩm

### API & Hook

**WordPress Hooks Used:**
```php
// Action Hooks
do_action('woocommerce_add_to_cart');
do_action('acf/save_post');

// Filter Hooks
apply_filters('woocommerce_product_get_price', $price);
apply_filters('woocommerce_cart_contents', $cart);
```

---

## 🧪 Kiểm Thử

### Tài Khoản Demo

| Vai Trò | Username | Password | Ghi Chú |
|---------|----------|----------|---------|
| **Admin** | `admin` | `admin123` | Quản trị website |
| **Khách Hàng** | - | - | Không cần đăng ký |

> ⚠️ **Bảo Mật:** Đổi mật khẩu ngay trong production!

### Test Cases

- ✅ Tìm kiếm sản phẩm theo từ khóa
- ✅ Lọc theo danh mục & giá
- ✅ Thêm sản phẩm vào giỏ hàng
- ✅ Cập nhật số lượng
- ✅ Thanh toán & nhận email xác nhận
- ✅ Chat với Chatbot AI
- ✅ Responsive trên mobile

---

## 📚 Tài Liệu Tham Khảo

### Chính Thức
- [WordPress Docs](https://wordpress.org/support/) - Tài liệu WordPress
- [PHP Manual](https://www.php.net/docs.php) - Hướng dẫn PHP
- [MySQL Docs](https://dev.mysql.com/doc/) - Tài liệu MySQL
- [WooCommerce Docs](https://woocommerce.com/documentation/) - WooCommerce

### Bài Viết Tham Khảo
- [WordPress Hooks & Filters](https://developer.wordpress.org/plugins/hooks/)
- [Custom Post Types](https://developer.wordpress.org/plugins/post-types/)
- [Advanced Custom Fields](https://www.advancedcustomfields.com/resources/)

---

## 🐛 Troubleshooting

### ❌ Database Connection Error
```php
// Kiểm tra wp-config.php
define('DB_NAME', 'wordpress_db');
define('DB_USER', 'root');
define('DB_PASSWORD', '');
define('DB_HOST', 'localhost');
```

### ❌ Plugin Không Kích Hoạt
```bash
# Tăng memory limit trong wp-config.php
define('WP_MEMORY_LIMIT', '256M');
```

### ❌ Email Không Gửi
```bash
# Cài plugin WP Mail SMTP
# Cấu hình SMTP server (Gmail, Sendgrid, v.v.)
# Settings → WP Mail SMTP
```

### ❌ Chatbot Không Hoạt Động
```bash
# Kiểm tra file custom-code/chatbot-ai.php
# Verify Ajax handlers đã đúng
# Check browser console for JS errors
```

---

## 🤝 Đóng Góp & Phát Triển

### Phiên Bản Hiện Tại
- **v1.0.0** - Stable (May 2026)

### Tính Năng Sắp Tới
- [ ] Tích hợp thanh toán online (PayPal, VNPay)
- [ ] Quản lý đơn hàng nâng cao
- [ ] Email marketing automation
- [ ] Mobile app native
- [ ] Analytics dashboard

### Cách Đóng Góp
1. Fork repository
2. Tạo branch feature: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -am 'Add feature'`
4. Push branch: `git push origin feature/your-feature`
5. Mở Pull Request

---

## 📄 License

Dự án này được thực hiện cho mục đích **học tập** trong học phần **"Phần mềm mã nguồn mở"**.

© 2026 **Đinh Quang Duy** & **Trần Quang Minh**  
Trường Đại Học Điện Lực - Khoa Công Nghệ Thông Tin

---

## 📞 Liên Hệ

- **Đinh Quang Duy** - [GitHub](https://github.com/mingdz217)
- **Trần Quang Minh** - [GitHub](https://github.com/tranquangminh)
- **Email:** duydinhquang@gmail.com
- **Website:** http://localhost (khi chạy local)

---

## 🙏 Lời Cảm Ơn

- ❤️ Cảm ơn **ThS. Cấn Đức Điệp** - Giảng viên hướng dẫn tận tâm
- ❤️ Cảm ơn **Đại Học Điện Lực** - Cung cấp cơ sở hạ tầng & hỗ trợ
- ❤️ Cảm ơn cộng đồng **WordPress** & **PHP** - Các tài liệu & plugin tuyệt vời

---

<div align="center">

### 🌟 Nếu dự án này hữu ích, hãy ⭐ Star Repository!

**Made with ❤️ by Duy & Minh**

</div>

---

## 📋 Changelog

### v1.0.0 (May 2026)
- ✅ Trang chủ giới thiệu sản phẩm
- ✅ Danh sách & chi tiết sản phẩm
- ✅ Tìm kiếm & lọc nâng cao
- ✅ Giỏ hàng & thanh toán
- ✅ Chatbot AI thông minh
- ✅ Gửi email xác nhận
- ✅ Responsive design
- ✅ Blog/Tin tức

---

**Last Updated:** May 2026  
**Status:** ✅ Active & Maintained

