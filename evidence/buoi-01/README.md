# Minh chứng Buổi 1

Thư mục này dùng để nộp minh chứng thiết lập môi trường lab.

## Sinh viên điền thông tin

- Họ tên: Võ Văn Quyền 
- Mã sinh viên: 1771020583
- Nhóm: 6
- Vai trò dự kiến trong nhóm:Backend Developer (phụ trách xây dựng API và xử lý dữ liệu)
- Hệ điều hành: Windows 10
- Ghi chú:Dùng Miniconda, Git và thiết lập môi trường thành công

## Các file minh chứng nên có

Các file minh chứng nên có
tool-versions.txt → chứa thông tin version của các công cụ (Node, Git, Docker...)
docker-version.txt → kết quả lệnh docker --version
compose-version.txt → kết quả lệnh docker-compose --version
hello-world.txt → kết quả chạy container hello-world
smoke-test-result.txt → kiểm tra hệ thống hoạt động
image-list.txt → danh sách Docker images (docker images)
git-log.txt → lịch sử commit (git log)
checklist.md → checklist hoàn thành
known-issues.md → các lỗi gặp phải
Cách sinh file tự động
Windows (PowerShell)
.\scripts\collect_session01_evidence.ps1
📌 Nội dung checklist.md (bạn có thể tạo file này)
# Checklist Buổi 1

- [x] Cài đặt Git
- [x] Cài đặt Docker
- [x] Cài đặt Docker Compose
- [x] Chạy thử container hello-world
- [x] Kiểm tra docker images
- [x] Clone repository thành công
- [x] Push code lên GitHub
⚠️ Nội dung known-issues.md
# Known Issues

## Lỗi 1: Git push bị lỗi "src refspec main does not match any"
- Nguyên nhân: Chưa commit file nào
- Cách fix:
  git add .
  git commit -m "first commit"
  git branch -M main
  git push -u origin main

## Lỗi 2: Docker không chạy
- Nguyên nhân: Chưa bật Docker Desktop
- Cách fix: Mở Docker Desktop trước khi chạy lệnh
📊 Liên hệ với đề tài A5
Service của nhóm

Hệ thống dịch vụ tổng hợp và phân tích dữ liệu sẽ:

✔ Service có trách nhiệm:
Thu thập dữ liệu từ nhiều nguồn (API, file, database)
Xử lý và làm sạch dữ liệu
Phân tích dữ liệu (thống kê, xu hướng)
Cung cấp API cho frontend hoặc hệ thống khác
❌ Service KHÔNG làm:
Không xử lý giao diện người dùng (frontend)
Không lưu trữ dữ liệu lâu dài (nếu dùng service riêng)
Không xử lý xác thực người dùng (nếu có auth service riêng)
