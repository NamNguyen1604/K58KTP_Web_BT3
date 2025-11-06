## K58KTP_Web_BT3
## Bài tập 3 : Nguyễn Phương Nam - K225480106092 
# Yêu cầu bài tập : LẬP TRÌNH ỨNG DỤNG WEB trên nền linux
1. Cài đặt môi trường linux: SV chọn 1 trong các phương án
2. Cài đặt Docker (nếu dùng docker desktop trên windows thì nó có ngay)
3. Sử dụng 1 file docker-compose.yml để cài đặt các docker container sau: 
4. Lập trình web frontend+backend:
 4.1 Web thương mại điện tử
 4.2 Web IOT: Giám sát dữ liệu IOT.
5. Nginx làm web-server
# Bài làm : 
BƯỚC 1 & 2: Cài Đặt Môi Trường (Linux + Docker)
Cài đặt Docker Desktop: Tải và cài đặt Docker Desktop (sử dụng WSL 2 làm backend).
<img width="943" height="850" alt="image" src="https://github.com/user-attachments/assets/d52a499b-7e3a-4807-905f-a1288ea87e8a" />
Kiểm tra: Đảm bảo WSL 2 đã được kích hoạt và Docker Desktop đang chạy
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/32dc21c8-da2c-41f2-a23d-25a4dd7715ce" />
BƯỚC 3: Tạo Stack Dịch Vụ (Docker Compose)
1. Chuẩn bị Thư mục : BTWEB
2. Cấu trúc File (Bắt buộc)
Tạo 3 thành phần sau trong thư mục dự án:
-File: docker-compose.yml
-File: nginx.conf
-Thư mục: frontend
+File: frontend/index.html
3. Chạy Stack
<img width="930" height="340" alt="image" src="https://github.com/user-attachments/assets/d046eb16-bb53-49e9-aac8-6b56886ef85f" />
BƯỚC 5: Cấu Hình Tên Miền (File Hosts)
Mở file: C:\Windows\System32\drivers\etc\hosts.
Thêm dòng sau vào cuối file:127.0.0.1   phuongnam.com xong lưu lại.
<img width="938" height="853" alt="image" src="https://github.com/user-attachments/assets/2a8feadf-b5cc-48c3-9a7a-938458af4685" />
BƯỚC 4: Lập Trình Backend (Node-RED & CSDL)
1. Cấu hình CSDL (MariaDB & InfluxDB)
- MariaDB: http://localhost:8080
 <img width="935" height="936" alt="image" src="https://github.com/user-attachments/assets/f7fea7ae-af4d-43bb-88fb-0e601f1754c5" />
<img width="1024" height="576" alt="image" src="https://github.com/user-attachments/assets/01766da7-9e4d-4c7a-b011-22bc5e3aade5" />
- InfluxDB:http://localhost:8086
<img width="1135" height="616" alt="image" src="https://github.com/user-attachments/assets/5977d6fa-eb75-4aeb-805d-ef36657a2099" />
2. Cài đặt Node-RED Modules
  Truy cập http://phuongnam.com/nodered/ $\rightarrow$ Manage palette $\rightarrow$ Install.
  Cài đặt: node-red-contrib-influxdb và node-red-contrib-mysql


  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f2f7cdc1-ff21-487e-acb6-b9c415585fbb" />


