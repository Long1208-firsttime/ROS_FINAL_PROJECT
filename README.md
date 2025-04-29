
---

# ASlAM ROBOT ROS

**SIX** là mô hình bài cuối kỳ ROS, file github này gồm những phần sau.

## 📁 Cấu trúc thư mục SIX

- `config/`: Chứa các tệp cấu hình cho robot và môi trường mô phỏng.
- `launch/`: Tập tin khởi động mô phỏng và các thành phần liên quan.
- `maps/`: Dữ liệu bản đồ sử dụng trong mô phỏng.
- `meshes/`: Tệp lưới 3D cho các mô hình robot và môi trường.
- `models/`: Mô hình robot và các đối tượng khác trong mô phỏng.
- `param/`: Các tệp thông số cấu hình cho robot và mô phỏng.
- `scripts/`: Tập lệnh điều khiển và hỗ trợ mô phỏng.
- `urdf/`: Tệp mô tả robot sử dụng định dạng URDF.
- `worlds/`: Tệp định nghĩa thế giới mô phỏng trong Gazebo hoặc môi trường tương tự.
- `CMakeLists.txt`: Tệp cấu hình xây dựng dự án.
- `package.xml`: Tệp mô tả gói ROS, bao gồm thông tin về phụ thuộc và metadata.

## 🚀 Yêu cầu hệ thống

- ROS (Robot Operating System) - phiên bản phù hợp với dự án.
- Gazebo hoặc môi trường mô phỏng tương thích.
- Python, Lua, và CMake để chạy các tập lệnh và xây dựng dự án.

## 🔧 Cài đặt

1. Clone kho lưu trữ:

   ```bash
   git clone https://github.com/hungne121/six.git
   ```

2. Cài đặt TEB.:
 http://wiki.ros.org/teb_local_planner/Tutorials/Setup%20and%20test%20Optimization

3. Cài đặt Gmapping:
     sudo apt update
     sudo apt install ros-noetic-slam-gmapping


## Khởi chạy cac file launch.
1. Chạy demo ASLAM với map đơn giản.

   roslaunch six explorer.launch
   
2. Chạy ASLAM hoặc Gmaping với các map phức tạp hơn.
a. Khởi chạy map.
   Map book_store: _roslaunch six bookstore.launch_

   Map frosland : _roslaunch six map_frostland.launch_

   Map park: _roslaunch six map_park.launch_

   Map rock: _roslaunch six map_rocklaunch_ 

   Map office: _roslaunch six office.launch_

b. Tự động khám phá.

_rosrun six test_1.py_

---

