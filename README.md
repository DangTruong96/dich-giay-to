# Dịch Giấy Tờ Việt – Nhật

Trang web tĩnh (HTML/CSS/JS thuần, không cần build) cho dịch vụ dịch giấy tờ Việt Nam sang tiếng Nhật:

- **Công cụ dịch miễn phí**: người dùng chọn loại giấy tờ, điền thông tin → nhận bản dịch tiếng Nhật theo mẫu chuẩn → in / lưu PDF. Công cụ chạy hoàn toàn trên trình duyệt, không gửi dữ liệu đi đâu.
- **Bài hướng dẫn SEO** về thủ tục giấy tờ cho người Việt tại Nhật.
- **Trang dịch vụ** giới thiệu dịch vụ dịch thuật có chứng thực (trả phí).

Trang chạy bằng GitHub Pages từ nhánh `main`, thư mục gốc.

## Cấu trúc thư mục

| File | Nội dung |
|---|---|
| `index.html` | Trang chủ: giới thiệu, danh sách loại giấy tờ, mục dịch vụ, ô quảng cáo, thẻ bài hướng dẫn |
| `cong-cu.html` | Công cụ dịch (được tạo từ ứng dụng dịch giấy tờ — **sẽ bổ sung sau**, hiện liên kết đã đặt sẵn) |
| `config.js` | **File cấu hình liên kết duy nhất** — xem mục dưới |
| `huong-dan-dich-giay-khai-sinh.html` | Bài hướng dẫn: dịch giấy khai sinh sang tiếng Nhật |
| `huong-dan-ket-hon-voi-nguoi-nhat.html` | Bài hướng dẫn: giấy tờ phía Việt Nam khi kết hôn với người Nhật |
| `chinh-sach-bao-mat.html` | Chính sách bảo mật |
| `lien-he.html` | Trang liên hệ / đặt dịch |

## Cách gắn link (Zalo, Facebook, quảng cáo)

Mở file **`config.js`** và điền link vào các ô tương ứng:

```js
window.SITE_CONFIG = {
  zaloUrl: "",       // ví dụ: "https://zalo.me/..."
  facebookUrl: "",   // link trang cá nhân hoặc fanpage
  affiliate1Url: "", // link quảng cáo / tiếp thị liên kết 1
  affiliate2Url: ""  // link quảng cáo / tiếp thị liên kết 2
};
```

- Ô nào để trống (`""`) thì nút / khung quảng cáo tương ứng **tự động ẩn** trên trang — không hiện nút chết.
- Sau khi sửa, commit và push lên GitHub, GitHub Pages sẽ tự cập nhật trang trong ít phút.
- Không cần sửa bất kỳ file HTML nào để đổi link.

## Ghi chú

- `cong-cu.html` do ứng dụng dịch giấy tờ xuất ra; khi có bản mới chỉ cần thay file đó vào thư mục này rồi push.
- Nội dung các bài hướng dẫn chỉ mang tính tham khảo chung, không phải tư vấn pháp lý.
