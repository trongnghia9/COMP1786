# Requirements Analysis - COMP1786 Hike Tracker Project

## Hiện trạng dự án

### ✅ Đã hoàn thành (React Native):
1. **Task e (10%)** - Enter Hike Details (React Native) - ✅ Hoàn thành
2. **Task f (10%)** - Cross-Platform Persistence (React Native) - ✅ Hoàn thành
3. **Task d (10%)** - Search Functionality (React Native) - ✅ Hoàn thành

### ⚠️ Thiếu các yêu cầu chính:
1. **Task a (10%)** - Enter Hike Details (Android Java) - ❌ Thiếu
2. **Task b (15%)** - Manage Hike Data (Android Java) - ❌ Thiếu
3. **Task c (15%)** - Add Hike Observations - ❌ Thiếu hoàn toàn
4. **Task g (10%)** - Additional Features - ❌ Thiếu

---

## Phân tích chi tiết theo yêu cầu

### ❌ Task a: Enter Hike Details (Android Java) - 10%
**Yêu cầu:**
- Tạo GUI để nhập thông tin hike
- Các trường bắt buộc: Name, Location, Date, Parking, Length, Difficulty
- Các trường tùy chọn: Description + 2 custom fields
- Validate input, hiển thị error messages
- Màn hình xác nhận cho phép review và edit

**Hiện trạng:** ❌ Thiếu hoàn toàn
- Không có ứng dụng Android Java
- Cần tạo project Android native

**Cần làm:**
1. Tạo project Android với Java
2. Tạo UI để nhập hike details
3. Implement validation
4. Tạo confirmation screen

---

### ❌ Task b: Manage Hike Data (Android Java) - 15%
**Yêu cầu:**
- Lưu tất cả hike details vào SQLite database
- Xem danh sách tất cả hikes
- Chọn hike để edit
- Xóa từng hike
- Option để xóa tất cả hikes (reset)

**Hiện trạng:** ❌ Thiếu hoàn toàn
- React Native version có các features này
- Cần tạo trong Android Java

**Cần làm:**
1. Setup SQLite database
2. Implement CRUD operations
3. Create list view
4. Implement edit functionality
5. Implement delete individual/all

---

### ❌ Task c: Add Hike Observations (Android Java) - 15%
**Yêu cầu:**
- Cho phép thêm một hoặc nhiều observations cho mỗi hike
- Mỗi observation cần: description, time (default current time), optional comments
- Lưu vào SQLite database
- Có thể view, edit, delete observations

**Hiện trạng:** ❌ Thiếu hoàn toàn
- Không có observations table trong database
- Không có UI để manage observations
- **Đây là requirement quan trọng bị thiếu hoàn toàn**

**Cần làm:**
1. Tạo observations table trong database (cả React Native và Android)
2. Tạo UI để add observations
3. Implement view/edit/delete observations
4. Link observations với hikes qua foreign key

---

### ✅ Task d: Search Functionality (Android Java) - 10%
**Hiện trạng:** ✅ Đã có trong React Native version
- Basic search: Tìm hike theo name
- Advanced search: Name, location, length, date
- Có thể select hike từ kết quả

**Cần làm:**
- Cần implement trong Android Java version

---

### ✅ Task e: Cross-Platform Prototype (React Native) - 10%
**Hiện trạng:** ✅ Hoàn thành
- EntryScreen.js implement task a với đầy đủ fields
- UI đẹp, có validation

---

### ✅ Task f: Cross-Platform Persistence (React Native) - 10%
**Hiện trạng:** ✅ Hoàn thành
- SQLite database hoạt động
- Có thể view, add, edit, delete hikes
- **Đã thêm: Edit hike functionality**

**Đã làm:**
1. ✅ Edit hike functionality đã được thêm

---

### ❌ Task g: Additional Features - 10%
**Yêu cầu:** Optional extension features
- Examples: Photos from camera, GPS location, Display on map, External web service

**Hiện trạng:** ❌ Chưa có
- Không có additional features nào

**Đề xuất implement:**
1. Add camera integration để chụp ảnh hikes
2. Add GPS để tự động lấy location
3. Hoặc add map view để hiển thị hike locations

---

## Tổng kết điểm

| Task | Điểm | Hiện trạng | %
|------|------|------------|---
| a) Enter Hike Details (Android Java) | 10% | ❌ Thiếu | 0%
| b) Manage Hike Data (Android Java) | 15% | ❌ Thiếu | 0%
| c) Add Hike Observations | 15% | ❌ Thiếu hoàn toàn | 0%
| d) Search (Android Java) | 10% | ✅ Có trong RN | 0%
| e) Cross-Platform Prototype | 10% | ✅ Hoàn thành | 10%
| f) Cross-Platform Persistence | 10% | ✅ Hoàn thành | 10%
| g) Additional Features | 10% | ❌ Thiếu | 0%

**Tổng điểm hiện tại: ~30/100 điểm**

---

## Những việc cần làm ngay

### 1. Priority HIGH - Task c (Observations) - 15%
**Thiếu hoàn toàn** - Đây là yêu cầu quan trọng bị bỏ sót hoàn toàn

Cần:
1. Tạo observations table trong database schema
2. Implement trong cả React Native VÀ Android
3. Create UI để add/edit/delete/view observations

### 2. Priority HIGH - Android Java App (Tasks a,b,d) - 35%
Cần tạo native Android app với:
- Enter hike details
- Manage hike data (CRUD)
- Search functionality

### 3. ✅ Priority MEDIUM - Edit Hike (React Native) - 2%
✅ Hoàn thành - Edit functionality đã được thêm vào React Native version

### 4. Priority MEDIUM - Task g (Additional Features) - 10%
Cần thêm ít nhất một advanced feature

---

## Khuyến nghị

**Để đạt đủ điểm:**
1. **Ngay lập tức:** Implement Task c (Observations) - thiếu hoàn toàn
2. **Quan trọng:** Tạo Android Java app để đáp ứng tasks a, b, d
3. ✅ **Bổ sung:** Đã thêm edit hike trong React Native
4. **Tùy chọn:** Thêm additional features (Task g)

**Thứ tự ưu tiên:**
1. Task c (Observations) - 15 điểm - Thiếu hoàn toàn
2. Tasks a, b, d (Android Java) - 35 điểm - Thiếu hoàn toàn
3. Edit hike (React Native) - 2 điểm
4. Task g (Additional Features) - 10 điểm
