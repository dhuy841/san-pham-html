# Mini Project: Trang chủ báo điện tử bằng CSS Grid

## Nội dung
- `index.html`: cấu trúc ngữ nghĩa của trang báo điện tử.
- `style.css`: CSS Grid tổng thể, nested grid, mosaic bất đối xứng và responsive.
- Các hình minh họa được tạo bằng CSS nên không cần tải thêm ảnh.

## Chạy thử trên máy
1. Giải nén thư mục dự án.
2. Mở thư mục `online-newspaper-grid` bằng VS Code.
3. Mở `index.html` trong trình duyệt, hoặc dùng tiện ích Live Server.
4. Thử thu nhỏ cửa sổ trình duyệt để kiểm tra giao diện responsive.

## Những yêu cầu CSS Grid đã áp dụng
- `.page-container`: `display: grid`, `grid-template-rows: auto 1fr auto`, `min-height: 100vh`.
- `.header` và `.footer`: `grid-column: 1 / -1`.
- `.content-grid`: nested grid với 4 cột, `grid-auto-rows` và `gap`.
- `.card-1`: `grid-column: span 2` và `grid-row: span 2`.
- `.card-2`: `grid-row: span 2`.
- `.card-5`: `grid-column: span 2`.
- Media queries giúp bố cục thích ứng trên máy tính bảng và điện thoại.

## Đẩy lên GitHub bằng Git Bash trong VS Code
Mở Terminal > New Terminal, đảm bảo terminal đang ở thư mục dự án, rồi chạy:

```bash
git init
git add .
git commit -m "Build responsive online newspaper homepage with CSS Grid"
```

Nếu bạn đã có repository GitHub:
1. Sao chép URL repository của bạn từ GitHub.
2. Chạy `git remote -v` để kiểm tra remote hiện có.
3. Nếu chưa có remote, chạy `git remote add origin URL_REPOSITORY_CUA_BAN`.
4. Kiểm tra nhánh với `git branch --show-current`.
5. Đẩy lên nhánh hiện tại, ví dụ `git push -u origin main`.

Nếu repository đã có sẵn lịch sử/commit, **không chạy `git init` hoặc đổi remote một cách tùy tiện**. Hãy mở đúng thư mục repository hiện tại, chép hai tệp `index.html` và `style.css` vào đó, sau đó chạy `git status`, `git add index.html style.css`, `git commit -m "Build online newspaper CSS Grid layout"` và `git push`.
