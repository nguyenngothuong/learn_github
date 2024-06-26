
# Quyết Tâm Học Git Bài Bản

Sau mấy năm trời học Git nhưng thực sự đây là lần tôi quyết tâm học đàng hoàng, làm ra project sử dụng với Git luôn cho thành thạo. Tôi đã note lại một vài nội dung quan trọng trong [Lark Docs](https://due-tmdt46k.larksuite.com/wiki/DLsrwB1U8itw9vkcutLuaY2ssoc?from=from_copylink) để chia sẻ lại kinh nghiệm cho mọi người.

## Nội Dung Quan Trọng

### 1. Các Nhánh Chính (The Main Branches)
- **Nhánh master**: Đây là nhánh chứa mã nguồn ở trạng thái sẵn sàng để triển khai. Mọi commit trên nhánh master đều có thể coi là một bản phát hành mới.
- **Nhánh develop**: Nhánh này chứa mã nguồn với những thay đổi và tính năng mới nhất cho bản phát hành tiếp theo. Nó còn được gọi là nhánh "integration".

### 2. Các Nhánh Hỗ Trợ (Supporting Branches)
- **Feature branches**:
  - Tách từ nhánh develop.
  - Dùng để phát triển các tính năng mới cho bản phát hành sắp tới hoặc trong tương lai.
  - Cuối cùng sẽ được hợp nhất trở lại vào nhánh develop.
  - Quy ước đặt tên: bất kỳ tên nào trừ master, develop, release-*, hotfix-*.
- **Release branches**:
  - Tách từ nhánh develop.
  - Dùng để chuẩn bị cho bản phát hành sản phẩm, cho phép sửa lỗi nhỏ và chuẩn bị các thông tin phiên bản.
  - Được hợp nhất vào cả nhánh master và develop khi hoàn tất.
  - Quy ước đặt tên: release-*.
- **Hotfix branches**:
  - Tách từ nhánh master.
  - Dùng để sửa nhanh các lỗi quan trọng trên phiên bản đang chạy.
  - Được hợp nhất vào cả nhánh develop và master.
  - Quy ước đặt tên: hotfix-*.

### 3. Quy Trình Làm Việc (Workflow)
1. Khi bắt đầu một tính năng mới, tạo một feature branch từ nhánh develop.
   ```sh
   # bước 1: move sang branch develop
   git checkout develop

   # bước 2: tạo feature từ develop
   git checkout -b feature/STT-tên issue hoặc tên tính feature cụ thể
   ```
2. Tạo code và fix :)))).

Tôi hy vọng những ghi chú này sẽ giúp ích cho các bạn trong quá trình học và làm việc với Git. Chúc các bạn thành công!