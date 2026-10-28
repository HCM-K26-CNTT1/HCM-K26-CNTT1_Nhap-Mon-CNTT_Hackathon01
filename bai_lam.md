# BÀI LÀM – HACKATHON 01

- **Mã đề:** 20
- **Họ tên:** Nguyễn Trần Đan Linh
- **Lớp:** CNTT1
- **Link repository:** https://github.com/HCM-K26-CNTT1/HCM-K26-CNTT1_Nhap-Mon-CNTT_Hackathon01.git
- **Hệ điều hành (Windows/macOS):** Windows

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
ls -la
mv lich_lam_viec.txt docs/
mv log0_salon_toc.PNG media/
rm temp_289.temp
cd logs/
cat log_salon.logs
cd ..

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
total 39
drwxr-xr-x 1 User 197121    0 Oct 28 07:43 ./
drwxr-xr-x 1 User 197121    0 Oct 28 07:39 ../
-rw-r--r-- 1 User 197121   67 Oct 27 01:32 .env
drwxr-xr-x 1 User 197121    0 Oct 28 07:40 backup/
-rw-r--r-- 1 User 197121 2230 Oct 27 01:32 bai_lam.md
drwxr-xr-x 1 User 197121    0 Oct 28 07:42 data/
drwxr-xr-x 1 User 197121    0 Oct 28 07:40 docs/
-rw-r--r-- 1 User 197121   62 Oct 27 01:32 lich_lam_viec.txt
-rw-r--r-- 1 User 197121 6113 Oct 27 01:32 logo_salon_toc.PNG
drwxr-xr-x 1 User 197121    0 Oct 28 07:42 logs/
drwxr-xr-x 1 User 197121    0 Oct 28 07:40 media/
-rw-r--r-- 1 User 197121   22 Oct 27 01:32 temp_289.tmp


```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
cd ..
D:
cd .\salon_toc_website\
Get-Content "logs\log_salon.log" | Select-String "ERROR" >> "logs\daily_report.txt"

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
2026-11-28 09:53:35 [ERROR] Khong tim thay trang /kieu-toc-moi (404)
2026-11-28 09:57:35 [ERROR] Khong tim thay trang /kieu-toc-moi (404)
```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.
> 
- [X] Heading 1: tên dự án
- [X] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [ ] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [X] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [X] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [X] Blockquote nhắc không upload `.env`


## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Scripts: auto_report.ps1
# Tac gia: Nguyễn Trần Đan Linh
# Ngay tao: 28/10/2026


@echo off
cd /d "%~dp0.."

if not exist "logs\log_salon.log" (
	echo Khong tim thay file log!
	pause
	exit
)
echo ===BAO CAO SU CO===>"logs\daily_report.txt"
findstr / I "ERROR" "logs\log_salon.log">> "logs\daily_report.txt"

echo Da tao bao cao
pause


```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/hoa_don_salon_thang_11.xlsx`, không cần ghi vào đây.
