# C

## Mục lục nội dung

- [1. Cookie](#1-cookie)

## 1. Cookie

**Quy trình hoạt động**

![cookie](/assets/cookie1.jpg)

**Một vài thuộc tính cookie**

![cookie](/assets/cookie2.jpg)

- Là một tệp văn bản nhỏ **chứa các thông tin** (ghi nhớ đăng nhập, theo dõi, quảng cáo,...) được **server gửi đến máy người dùng**. Browser sẽ lưu trữ và **gửi lại server** mỗi khi **người dùng request** đến server.
  - Nếu một cookie không set thời gian tồn tại mặc định nó sẽ bằng session
  - Nếu **`HttpOnly`** set bằng false thì chúng ta có thể truy cập **`document.cookie`** trên console devtool lúc này có thể xem cookie **`==>`** không nên set **`HttpOnly`** bằng **`false`** vì có thể dẫn đến tấn công XSS
- Dung lượng tối đa là 4kb
- **hash-based token (cookie) ==>** token được tạo ra bằng cách mã hóa thông tin user thành một chuỗi hash và ghi vào cookie của trình duyệt. Cách này sẽ nhanh và đơn giản nhưng không an toàn
- **persistent token (cookie + database) ==>** token được lưu trữ trong cơ sở dữ liệu của ứng dụng. Cách này sẽ chậm nhưng an toàn hơn
- **`JSESSSIONID`** cookie, do java web application tạo ra, là một cookie lưu trữ **SessionID**, cookie này sẽ hết hạn khi đóng browser

**[⬆ Quay trở lại đầu trang](#mục-lục-nội-dung)**