# QR Code Login with Digital Signature (Demo)

## Giới thiệu

Đây là dự án demo hệ thống đăng nhập đa thiết bị sử dụng mã QR kết hợp với chữ ký số nhằm nâng cao bảo mật và tiện lợi trong xác thực người dùng.

Mục tiêu của dự án là xây dựng một cơ chế trong đó:

- Web app tạo mã QR chứa thông tin phiên đăng nhập.
- Mobile app đã đăng nhập quét mã QR, ký số thông tin phiên bằng khóa riêng (private key).
- Backend server xác minh chữ ký số để xác thực và cho phép đăng nhập trên thiết bị khác.

---

## Hiện trạng dự án

Hiện tại, dự án đang trong giai đoạn hoàn thiện phần lý thuyết của báo cáo nghiên cứu trước khi tiến hành triển khai thực tế các thành phần Web, Mobile và Backend.

---

## Các thành phần dự kiến

| Thành phần     | Công nghệ đề xuất                 | Vai trò                                             |
|----------------|---------------------------------|----------------------------------------------------|
| Web Frontend   | React / HTML/JavaScript          | Tạo mã QR chứa session đăng nhập                    |
| Mobile App     | Flutter / React Native / Android | Quét mã QR, ký số phiên đăng nhập                   |
| Backend Server | Node.js / Python Flask / Express | Quản lý phiên đăng nhập và xác minh chữ ký số      |
| Mã hóa         | RSA (2048 bit) hoặc ECDSA         | Tạo và xác minh chữ ký số                            |

---

## Quy trình hoạt động dự kiến

1. Người dùng mở web, server tạo một session đăng nhập và trả về mã QR chứa session ID.
2. Mobile app quét mã QR, tạo chữ ký số trên session ID bằng khóa riêng của người dùng.
3. Mobile app gửi chữ ký số và thông tin liên quan về server.
4. Server xác minh chữ ký, nếu hợp lệ thì xác nhận phiên đăng nhập.
5. Web app nhận thông báo và cho phép truy cập.

---

## Lợi ích học tập

- Thực hành kỹ thuật mật mã học nâng cao (chữ ký số).
- Tích hợp giữa web, mobile và backend.
- Áp dụng cho hệ thống đăng nhập an toàn, không cần mật khẩu.

---

## Liên hệ

Mọi thắc mắc hoặc góp ý, vui lòng liên hệ: [lehoangthan584@gmail.com](mailto:lehoangthan584@gmail.com)

---

*Lưu ý: Đây là bản demo ý tưởng, chưa triển khai hoàn chỉnh.*
