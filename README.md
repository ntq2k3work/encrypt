# Enrypt_An_toan_thong_tin
## Ceaser
    Giải thích cách hoạt động:
        + Cho 1 plaintext và 1 key số nguyên
        + Sử dụng bảng chữ cái tiếng anh để mã hoá (Từ a -> z)
        + Mã hoá bằng cách thay thế ký tự trong plaintext bằng (ký tự đó + key) mod 26 
    Ví dụ :
        + plaintext = 'abc' , key = 3
        + Encrypt plaintext : 'abc' -> 'def' 
        + (a + 3) % 26 = d | (b + 3) % 26 = e | (c + 3) % 26 = f
    Nhược điểm :
        + Không mã hoá được tiếng việt,unicode
        + Dễ bị bắt bài khi chạy for