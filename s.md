# S

## Mục lục nội dung

- [1. Session](#1-session)
- [2. Session storage](#2-session-storage)

## 1. Session

**Quy trình hoạt động**

![session](/assets/session.jpg)

- Một session bắt đầu khi client gửi request đến server
- Nó tồn tại xuyên suốt từ trang này đến trang khác trong ứng dụng web
- Mất khi hết thời gian timeout hoặc khi bạn đóng ứng dụng.
- Giá trị của session sẽ được lưu trong một file trên server
- Là 1 vùng nhớ trên ram server

**[⬆ Quay trở lại đầu trang](#mục-lục-nội-dung)**

## 2. Session storage

- Là một feature mới của HTML5 cho phép lưu trữ bất kì info trong browser dùng JavaScript
- Dung lượng tối đa 5mb
- Khi đóng tab hay browser sẽ mất data
- Lưu data theo cặp key/value ở browser và server không access được các data này.
- Chỉ lưu 1 String, các kiểu data phức tạp không phù hợp để lưu
- Có thể bị đọc bởi js và xoá thông qua js hoặc thủ công

**[⬆ Quay trở lại đầu trang](#mục-lục-nội-dung)**