Phần 1 - Phân tích logic:

Mặc định, @CookieValue yêu cầu Cookie phải tồn tại (required = true).

Nếu khách mới chưa có Cookie, Spring sẽ ném MissingRequestCookieException ngay trước khi chạy vào nội dung hàm. Do đó, dòng if (guestName == null) sẽ không bao giờ được thực thi.
