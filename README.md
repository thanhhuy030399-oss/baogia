# Ứng dụng Báo giá nội thất (PWA): hướng dẫn cài đặt

## Trong gói có gì
- `index.html`: toàn bộ ứng dụng
- `manifest.json`: thông tin để điện thoại nhận đây là một app (tên, biểu tượng, màu)
- `sw.js`: giúp app chạy được khi không có mạng
- ``: biểu tượng app

## Bước 1: Đưa lên GitHub Pages (miễn phí, khoảng 10 phút, làm một lần)
1. Tạo tài khoản ở https://github.com (nếu chưa có).
2. Bấm dấu **+** ở góc trên → **New repository**.
   - Repository name: `baogia` (hoặc tên khác, viết liền không dấu)
   - Chọn **Public** → bấm **Create repository**.
3. Trong trang repository vừa tạo, bấm **uploading an existing file**.
4. Giải nén file zip, rồi kéo **tất cả** các file và các file ảnh biểu tượng vào ô tải lên.
   Bấm **Commit changes**.
5. Vào **Settings** → **Pages** (menu bên trái).
   - Source: **Deploy from a branch**
   - Branch: **main**, thư mục **/(root)** → bấm **Save**.
6. Đợi 1–2 phút, tải lại trang. Link app hiện ở đầu mục Pages, dạng:
   `https://ten-tai-khoan.github.io/baogia/`

## Bước 2: Cài lên điện thoại và máy tính
- **iPhone:** mở link bằng **Safari** → nút Chia sẻ → **Thêm vào MH chính**.
- **Android:** mở link bằng **Chrome** → bấm **Cài ứng dụng** trên đầu trang, hoặc ⋮ → **Cài đặt ứng dụng**.
- **Máy tính (Chrome/Edge):** bấm **Cài ứng dụng** trên đầu trang, hoặc biểu tượng cài đặt ở thanh địa chỉ.

## Lưu ý quan trọng về dữ liệu
- Bảng giá, mẫu thương hiệu, lịch sử báo giá và ảnh được **lưu ngay trên từng máy**.
  Điện thoại và máy tính **không tự đồng bộ** với nhau.
- Để chuyển dữ liệu sang máy khác: tab **Bảng giá** → **Tải file sao lưu**, gửi file đó sang máy kia
  (Zalo, email, Google Drive), rồi bấm **Khôi phục từ file**.
- **Nên sao lưu định kỳ.** Nếu xóa app hoặc xóa dữ liệu trình duyệt thì dữ liệu trên máy đó sẽ mất.
- Trên iPhone, dữ liệu của app cài ngoài màn hình chính tách riêng với Safari. Hãy dùng app từ biểu tượng ngoài màn hình chính.

## Cập nhật app sau này
Khi có bản `index.html` mới: vào repository trên GitHub → **Add file** → **Upload files** → kéo file mới vào → **Commit changes**.
Dữ liệu trên các máy **không bị mất** khi cập nhật. Mở app có mạng một lần là nhận bản mới.

## Khác với bản chạy trong Claude
- Không cần tài khoản Claude, mở toàn màn hình như app thật, dùng được khi không có mạng.
- Không có nút **Google Sheet** (cần kết nối của Claude). Bạn có thể **Xuất Excel** rồi mở file đó bằng Google Sheets.
- Dữ liệu không dùng chung giữa nhân viên. Mỗi người có dữ liệu riêng trên máy mình.
