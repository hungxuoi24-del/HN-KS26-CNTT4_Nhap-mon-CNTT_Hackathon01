# BÀI LÀM – HACKATHON 01

- **Mã đề:** 02
- **Họ tên:** Nguyễn Duy Hưng
- **Lớp:** HNKS26-CNTT4
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** Windown

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
1. Hiển thị đường dẫn tuyệt đối của thư mục hiện tại.
    - pwd

2. Liệt kê nội dung, gồm cả file ẩn. 
    - ls [-Force]

3. Di chuyển các file cong_thuc.txt vào docs, các file logo vào media.
    - mv .\Cong_Thuc.txt .\docs\
    - mv .\Logo_Tiem_Banh.PNG .\media\

4. Sao chép logo từ media vào backup.
    - cp .\media\Logo_Tiem_Banh.PNG .\backup\

5. Xoá file .tmp tại thư mục gốc; không xoá file khác.
    - rm .\temp_027.tmp

6. Dùng đường dẫn tương đối vào logs, liệt kê nội dung rồi quay lại thư mục gốc.
    -  Get-Content .\logs\Web.log
    - cd ..

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text


```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
1. Dùng các lệnh đọc file và lọc nội dung, tiến hành lọc các dòng chứa ERROR trong logs/web.log.
    -  Get-Content .\logs\Web.log | Select-String "ERROR"

2. Ghi kết quả vào logs/daily_report.txt.
    - Get-Content .\logs\Web.log | Select-String "ERROR" > .\logs\daily_report.txt
```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
2025-08-28 09:15:17 [ERROR] Loi ket noi cong thanh toan
2025-08-28 09:19:17 [ERROR] Loi ket noi cong thanh toan

```

## 4.4. Thao tác với tài liệu Markdown  


# Nhập môn công nghệ thông tin

***Ngành sử dụng máy tính, mạng và phần mềm để tự động hóa việc thu thập, xử lý, lưu trữ và truyền tải thông tin số.***

|Trí tuệ nhân tạo | Lập trình web | Lập trình app | An toàn thông tin 
| :--: | :--: | :--: | :--: |
| Chatbot LLM | Frontend React | IOS Swift | Kiểm thử thâm nhập |
| Nhận diện ảnh | Backend Node/Java | Android | Phòng chống mã độc |
| Dự báo số liệu | Sàn TMĐT | Flutter đa nền | Mã hóa dữ liệu |

```PowerShell
    ls
``` 

- [x] Xem elearning.

- [ ] Làm bài tập về nhà.

> không upload .env.


## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
- New_Item auto_report.ps1
- Get-Content logs\web.log | Select-String "ERROR" >> .\logs\auto_report.txt

```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
Đếm số dòng chứa ERROR trong logs/web.log bằng pipeline (dấu |) kết hợp các lệnh.
    - (Get-Content .\logs\Web.log | Select-String "ERROR").Count
```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
    5

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
Dòng đầu tiên: === TONG HOP LOG ===
  - "=== TONG HOP LOG ===" > logs/tong_hop.txt

Tiếp theo: các dòng chứa WARNING trong logs/web.log
  - Get-Content logs/web.log | Select-String "WARNING" >> logs/tong_hop.txt

Cuối cùng: số dòng chứa ERROR trong logs/web.log.
  - (Get-Content logs/web.log | Select-String "ERROR").Count >> logs/tong_hop.txt

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Excel


