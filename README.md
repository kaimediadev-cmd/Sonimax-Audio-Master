# SoniMax Audio Master 2026 - Enterprise Edition

Phần mềm chuyên dụng cao cấp can thiệp, tinh chỉnh DSP & đóng gói Firmware mạch loa kéo chuyên nghiệp.

![Platform](https://img.shields.io/badge/Platform-Windows%20x64-blue)
![Framework](https://img.shields.io/badge/.NET%20Framework-4.0%2B-green)
![Security](https://img.shields.io/badge/Security-SoniMax%20Guard%20Native%20x64-purple)
![Version](https://img.shields.io/badge/Version-2026.2.4-orange)

---

## 📥 Tải về trực tiếp (Download)

- 📦 **[Tải trọn bộ SoniMax_AudioMaster_2026_Enterprise.zip](https://github.com/kaimediadev-cmd/Sonimax-Audio-Master/raw/main/SoniMax_AudioMaster_2026_Enterprise.zip)** *(Khuyên dùng - Đầy đủ công cụ và thư viện)*
- ⚡ **[Tải riêng file SoniMaxAudioMaster.exe](https://raw.githubusercontent.com/kaimediadev-cmd/Sonimax-Audio-Master/main/SoniMaxAudioMaster.exe)**

---

## 🚀 Tính năng nổi bật

### 1. Hỗ trợ đa nền tảng chip vi điều khiển âm thanh
- **Dòng JieLi:** AC695N, AC696N (Định dạng file nạp: .ufw).
- **Dòng Bluetrum:** JX5918, H17N, T400S, T450S, V450S, V9033S, DSP-21X (Định dạng file nạp: .upd).

### 2. Tự động nhận diện Tên Bluetooth & Mã khóa chip
- **JieLi (.ufw):** Tự động bóc tách Tên Bluetooth gốc và Mã khóa chip (Chipkey 0x2606) từ phân vùng cfg_tool.bin và tail.bin.
- **Bluetrum (.upd):** Tự động nhận diện Tên Bluetooth và Mật khẩu phần cứng bảo vệ nạp mạch.
- Hỗ trợ đổi tên Bluetooth tiếng Việt có dấu chuẩn UTF-8 (tối đa 31 bytes).

### 3. Tính năng Bóc tách EQ / DSP hai chiều độc quyền (Reverse EQ Extraction)
- **Bóc EQ từ JieLi (.ufw):** Trích xuất cấu hình phần cứng DSP KT0708 (eq_cfg_hw.bin) thành mã nguồn C chuẩn (file mốc 	ruoc.c) để so sánh và tinh chỉnh với sau.c.
- **Bóc EQ từ Bluetrum (.upd):** Trích xuất toàn bộ các tệp group_0.bin -> group_5.bin ra thư mục riêng, cho phép kéo thả vào Audio WorkBench để xem & chỉnh sửa âm sắc gốc của các hãng loa.

### 4. Tinh chỉnh DSP & Cân chỉnh EQ chuyên sâu
- **JieLi:** Tinh chỉnh DSP KT0708 thông qua cặp file mốc 	ruoc.c và sau.c, hỗ trợ đồng bộ cả 2 preset phần cứng.
- **JX5918:** Tự động nhận diện các đời mạch:
  - *Đời Mới 2026 FBX 2 Chức Năng:* Hỗ trợ nạp 5 Mode Hát riêng biệt (group_1.bin -> group_5.bin) & 3 cấp chống hú.
  - *Đời V9033S / V5022S:* Hỗ trợ 3 Group DSP (group_0.bin -> group_2.bin).
  - *Đời 1 Group Cố Định:* V450S / T600S / V102L (group_0.bin).
  - Hỗ trợ nút đồng bộ nhanh 1 file .bin cho toàn bộ các Mode đang kích hoạt.

### 5. Thay thế & Chuẩn hóa âm thanh thông báo MP3
- Tự động gọt khoảng lặng sạch sẽ 2 đầu và nén vừa khít dung lượng slot Flash gốc (Zero-Overflow).
- Tùy biến âm Khởi động, Đã kết nối Bluetooth, Ngắt kết nối và các câu đọc AUX, Optical, USB, FM, Mic Priority...

### 6. Bảo mật & An toàn tuyệt đối (Zero-Brick)
- Kiểm soát 6 lớp thuật toán CRC16 & Cipher của JieLi.
- Phân tích và bảo vệ toàn vẹn bảng chỉ mục Jlfs & Info Table của Bluetrum.
- Tích hợp lớp bảo vệ **SoniMax Guard Native C++ x64** chống can thiệp bộ nhớ và khóa bản quyền theo HWID máy tính.
- Tích hợp hệ thống kiểm tra và cập nhật tự động (**Auto-Update**) trực tiếp từ máy chủ & GitHub.

---

## 📦 Bộ tệp tin chương trình

Để chương trình hoạt động ổn định, gói cài đặt gồm:
1. SoniMaxAudioMaster.exe : File thực thi chính của phần mềm (đã tích hợp icon logo & chứng thực phiên bản).
2. HUONG_DAN_SU_DUNG.txt : Tài liệu hướng dẫn sử dụng chi tiết.
3. Thư mục core/ : Chứa các thư viện phụ trợ hệ thống (SoniMaxGuard.dll, fmpeg.exe).

---

## 🔑 Kích hoạt bản quyền

1. Khởi động SoniMaxAudioMaster.exe.
2. Hộp thoại Đăng Nhập Hệ Thống xuất hiện. Bấm nút **[Sao chép]** tại ô **Mã nhận diện máy (HWID)**.
3. Gửi mã HWID và Gmail của bạn cho Quản trị viên để kích hoạt tài khoản.
4. Đăng nhập và bắt đầu sử dụng.

---

## 📄 Bản quyền
Bản quyền thuộc về **SoniMax Audio Master 2026**.
Mọi thông tin hỗ trợ kỹ thuật và đăng ký bản quyền vui lòng liên hệ Quản trị viên.