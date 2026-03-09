# 🌟 Portfolio Website - Thiên

Portfolio website cá nhân với thiết kế hiện đại, responsive và nhiều hiệu ứng tương tác.

![Portfolio Preview](https://via.placeholder.com/1200x600/667eea/ffffff?text=Portfolio+Website)

## ✨ Tính năng

- 🎨 **Thiết kế hiện đại**: Giao diện đẹp mắt với gradient màu sắc
- 📱 **Responsive**: Hoạt động tốt trên mọi thiết bị (desktop, tablet, mobile)
- 🎭 **Animations**: Hiệu ứng mượt mà khi scroll và hover
- 🎯 **Sections đầy đủ**:
  - Hero section với giới thiệu
  - About - Giới thiệu về bản thân
  - Skills - Kỹ năng với thanh progress bar
  - Projects - Danh sách dự án với overlay
  - Contact - Form liên hệ
- 🌐 **Smooth scrolling**: Cuộn mượt giữa các sections
- 📊 **Skill progress bars**: Thanh tiến trình kỹ năng animate
- 💌 **Contact form**: Form liên hệ với validation
- 🎨 **Cursor effect**: Hiệu ứng cursor tùy chỉnh
- 📈 **Progress bar**: Thanh tiến trình cuộn trang

## 🛠️ Công nghệ sử dụng

- **HTML5**: Cấu trúc semantic
- **CSS3**: Flexbox, Grid, Animations, Gradients
- **JavaScript**: Vanilla JS (không dùng framework)
- **Font Awesome**: Icons

## 📂 Cấu trúc thư mục

```
hi/
├── index.html      # File HTML chính
├── style.css       # File CSS styling
├── script.js       # File JavaScript
└── README.md       # File hướng dẫn này
```

## 🚀 Cách sử dụng

### 1. Mở trực tiếp

Chỉ cần double-click vào file `index.html` để mở trong browser.

### 2. Sử dụng Live Server (VS Code)

```bash
# Cài đặt Live Server extension trong VS Code
# Sau đó right-click vào index.html > Open with Live Server
```

### 3. Sử dụng Python simple server

```bash
# Python 3
python -m http.server 8000

# Sau đó mở: http://localhost:8000
```

## 🎨 Tùy chỉnh

### Thay đổi màu sắc

Mở file `style.css` và chỉnh sửa các biến CSS:

```css
:root {
    --primary-color: #667eea;     /* Màu chính */
    --secondary-color: #764ba2;   /* Màu phụ */
    --accent-color: #f093fb;      /* Màu nhấn */
    --text-dark: #2d3748;         /* Màu chữ tối */
    --text-light: #718096;        /* Màu chữ sáng */
}
```

### Thay đổi nội dung

1. **Thông tin cá nhân**: Sửa trong file `index.html`
   - Tên, tiêu đề trong hero section
   - Giới thiệu trong about section
   - Email, số điện thoại trong contact section

2. **Kỹ năng**: Thêm/sửa skill cards trong skills section

3. **Dự án**: Thêm/sửa project cards trong projects section

### Thêm ảnh cá nhân

Thay thế `.image-placeholder` trong about section:

```html
<!-- Thay đổi từ: -->
<div class="image-placeholder">
    <i class="fas fa-user"></i>
</div>

<!-- Thành: -->
<img src="your-photo.jpg" alt="Your Name" style="width: 300px; height: 300px; border-radius: 50%; object-fit: cover;">
```

### Thêm ảnh dự án

Thay thế `.project-placeholder` trong project cards:

```html
<!-- Thay đổi từ: -->
<div class="project-placeholder">
    <i class="fas fa-laptop-code"></i>
</div>

<!-- Thành: -->
<img src="project-image.jpg" alt="Project Name" style="width: 100%; height: 100%; object-fit: cover;">
```

## 🔗 Cập nhật links

### Social media links

Trong file `index.html`, tìm và cập nhật các links:

```html
<!-- Hero Section -->
<div class="social-links">
    <a href="https://github.com/your-username" target="_blank"><i class="fab fa-github"></i></a>
    <a href="https://linkedin.com/in/your-profile" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://facebook.com/your-profile" target="_blank"><i class="fab fa-facebook"></i></a>
    <a href="https://instagram.com/your-username" target="_blank"><i class="fab fa-instagram"></i></a>
</div>
```

### Project links

Cập nhật links trong project cards:

```html
<div class="project-overlay">
    <a href="https://your-project-demo.com" class="project-link"><i class="fas fa-external-link-alt"></i></a>
    <a href="https://github.com/your-username/project" class="project-link"><i class="fab fa-github"></i></a>
</div>
```

## 📧 Thiết lập Contact Form

Form hiện tại chỉ hiển thị notification. Để gửi email thật:

### Option 1: Formspree (miễn phí, dễ dùng)

1. Đăng ký tại [formspree.io](https://formspree.io)
2. Tạo form mới và lấy endpoint
3. Sửa form trong `index.html`:

```html
<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <input type="text" name="name" placeholder="Tên của bạn" required>
    <input type="email" name="email" placeholder="Email của bạn" required>
    <input type="text" name="subject" placeholder="Chủ đề" required>
    <textarea name="message" rows="5" placeholder="Nội dung tin nhắn" required></textarea>
    <button type="submit" class="btn btn-primary">Gửi tin nhắn</button>
</form>
```

### Option 2: EmailJS (miễn phí, không cần backend)

1. Đăng ký tại [emailjs.com](https://www.emailjs.com)
2. Thêm EmailJS script trong `index.html`:

```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
```

3. Cập nhật JavaScript để gửi email

## 🎯 Sections chi tiết

### 1. Hero Section
- Giới thiệu tên và vai trò
- Call-to-action buttons
- Social media links
- Scroll down indicator

### 2. About Section
- Ảnh đại diện
- Mô tả ngắn gọn
- Thông tin liên hệ
- Button CTA

### 3. Skills Section
- Grid hiển thị kỹ năng
- Icons cho mỗi kỹ năng
- Progress bars animate
- Percentage display

### 4. Projects Section
- Grid responsive cho dự án
- Project cards với hover effect
- Overlay với links
- Tags công nghệ

### 5. Contact Section
- Thông tin liên hệ
- Form với validation
- Icons cho thông tin
- Social links

## 🎨 Hiệu ứng đặc biệt

1. **Navbar scroll effect**: Navbar thay đổi khi scroll
2. **Smooth scrolling**: Cuộn mượt giữa sections
3. **Fade in animations**: Elements fade in khi vào viewport
4. **Skill bars animation**: Progress bars animate khi visible
5. **Hover effects**: Cards nổi lên khi hover
6. **Custom cursor**: Cursor tùy chỉnh (desktop)
7. **Page progress**: Thanh tiến trình ở top
8. **Parallax effect**: Hero background parallax

## 📱 Responsive Breakpoints

- **Desktop**: > 768px (full layout)
- **Tablet**: 768px (adjusted grid)
- **Mobile**: < 480px (single column)

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ⚠️ IE11 (limited support)

## 📝 Checklist tùy chỉnh

- [ ] Đổi tên và thông tin cá nhân
- [ ] Cập nhật email và số điện thoại
- [ ] Thêm ảnh đại diện
- [ ] Cập nhật social media links
- [ ] Thêm/sửa skills
- [ ] Thêm projects với ảnh và links
- [ ] Thêm ảnh cho projects
- [ ] Thiết lập form gửi email
- [ ] Đổi màu sắc (nếu muốn)
- [ ] Test trên mobile devices
- [ ] Deploy lên hosting

## 🚀 Deploy

### GitHub Pages (Miễn phí)

1. Tạo repository mới trên GitHub
2. Push code lên repository
3. Settings > Pages > Source: main branch
4. Website sẽ có địa chỉ: `https://your-username.github.io/repository-name`

### Netlify (Miễn phí)

1. Đăng ký tại [netlify.com](https://www.netlify.com)
2. Drag & drop folder vào Netlify
3. Website tự động deploy với domain miễn phí

### Vercel (Miễn phí)

1. Đăng ký tại [vercel.com](https://vercel.com)
2. Import từ GitHub hoặc drag & drop
3. Auto deploy khi có thay đổi

## 🐛 Troubleshooting

### Icons không hiển thị
- Kiểm tra kết nối internet (Font Awesome từ CDN)
- Thử thêm CDN backup:
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
```

### Animations không hoạt động
- Kiểm tra JavaScript đã load chưa
- Mở Console (F12) xem có lỗi không

### Form không gửi được
- Cần thiết lập backend hoặc dùng service (Formspree, EmailJS)
- Hiện tại form chỉ hiển thị notification

## 💡 Tips

1. **SEO**: Thêm meta tags trong `<head>`
2. **Performance**: Optimize images trước khi upload
3. **Accessibility**: Đảm bảo có alt text cho images
4. **Analytics**: Thêm Google Analytics để track visitors
5. **Favicon**: Thêm favicon.ico cho website

## 📄 License

Free to use for personal and commercial projects.

## 👤 Author

**Thiên**
- Portfolio: [Địa chỉ website của bạn]
- GitHub: [@your-username](https://github.com/your-username)
- Email: your.email@example.com

---

⭐ Nếu bạn thích project này, đừng quên star repo nhé!

Made with ❤️ and ☕ by Thiên
