
---


# 🤖 ASLAM ROBOT ROS – Dự án ROS cuối kỳ

**SIX** là mô hình mô phỏng cho bài cuối kỳ môn Robot Operating System (ROS). Repository này chứa toàn bộ mã nguồn, cấu hình và tập lệnh liên quan.

---

## 📁 Cấu trúc thư mục

- `config/` – Cấu hình cho robot và môi trường mô phỏng.
- `launch/` – Các file `.launch` dùng để khởi chạy hệ thống.
- `maps/` – Dữ liệu bản đồ cho mô phỏng.
- `meshes/` – File lưới 3D cho mô hình robot và đối tượng.
- `models/` – Mô hình robot và vật thể dùng trong môi trường.
- `param/` – Thông số cấu hình cho robot.
- `scripts/` – Các tập lệnh Python điều khiển hành vi robot.
- `urdf/` – Mô tả robot sử dụng định dạng URDF.
- `worlds/` – Thế giới mô phỏng dùng cho Gazebo.
- `CMakeLists.txt` – Tệp cấu hình build hệ thống.
- `package.xml` – Thông tin gói ROS và phụ thuộc.

---

## 🚀 Yêu cầu hệ thống

- ROS Noetic (hoặc phiên bản tương thích).
- Gazebo (hoặc môi trường mô phỏng tương thích).
- Python, Lua, CMake.

---

## 🔧 Cài đặt

1. **Clone repository:**

   ```bash
   git clone https://github.com/hungne121/six.git
   cd six
   ```

2. **Cài đặt TEB local planner:**

   Hướng dẫn tại: [TEB Setup Tutorial](http://wiki.ros.org/teb_local_planner/Tutorials/Setup%20and%20test%20Optimization)

3. **Cài đặt GMapping:**

   ```bash
   sudo apt update
   sudo apt install ros-noetic-slam-gmapping
   ```

---

## ▶️ Khởi chạy mô phỏng

### 1. Chạy demo ASLAM với bản đồ đơn giản:

```bash
roslaunch six explorer.launch
```

### 2. Chạy ASLAM hoặc GMapping với bản đồ phức tạp hơn:

#### a. Khởi chạy bản đồ:

- **Bookstore:**  
  ```bash
  roslaunch six bookstore.launch
  ```

- **Frostland:**  
  ```bash
  roslaunch six map_frostland.launch
  ```

- **Park:**  
  ```bash
  roslaunch six map_park.launch
  ```

- **Rock:**  
  ```bash
  roslaunch six map_rock.launch
  ```

- **Office:**  
  ```bash
  roslaunch six office.launch
  ```

#### b. Khám phá tự động:

```bash
rosrun six test_1.py
```

---

