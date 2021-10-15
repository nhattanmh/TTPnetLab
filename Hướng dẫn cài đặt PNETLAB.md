# MỤC LỤC
&ensp;[1, Tìm hiểu về PNET LAB](#1)

&ensp;[1.1,	Giới thiệu](#1.1)

&ensp;[1.2.	Mode PNETLAB](#1.2)

&ensp;[1.3.	Ưu điểm](#1.3) 

&ensp;[2. Cài đặt PnetLab trên VMWare](#2)


# <a name ="1">1.  Tìm hiểu về PNET LAB</a>
## <a name ="1.1">1.1.  Tìm hiểu về PNET LAB</a>
1.1	Giới thiệu:
-	PNETLAB hay được gọi là Packet Network Tool Lab, đây là 1 công cụ dung để giả lập các thiết bị mạng nhằm phục vụ cho mục đích học, thực hành, nghiên cứu thông qua giao diện quản trị câu lệnh (CLI) hoặc quản trị đồ họa (GUI).
+	Các nền tảng ảo hóa hỗ trợ:
-	VMware Workstation 12.5 trở lên
-	VMware Player 12.5 trở lên
-	VMware ESXi 6.0 trở lên
-	Ubuntu Server 16.04 LTS làm nền tảng cho kim loại trần (lộ trình)
-	Nền tảng đám mây của Google

## <a name ="1.2">1.2.  Mode PNETLAB</a>
-	PNETLAB có 2 chế độ: Offline Mode và Online Mode.
	
![image](https://user-images.githubusercontent.com/59860781/137438515-08817412-bbb5-473a-8dc8-d611a1637f64.png)

| Offline Mode  | Online Mode |  
| :----- | :---------- | 
| - Không cần internet để làm việc   | - Cần internet để làm việc.       |
| - Không cần đăng ký    | - 	Cần đăng ký.        | 
| -	Hỗ trợ đầy đủ các chức năng của PNETLab.   |-	Hỗ trợ đầy đủ các chức năng của PNETLab        |
| - Không thể chia sẻ hoặc bán lab cho PNETLAB Strore.    |- Có thể tải xuống và sử dụng tất cả các Lab trên Store.           | 
| - Giới hạn 10 tài khoản (Có thể nâng cấp nhưng cần có internet).   | - 	Có thể chia sẻ hoặc bán lab cho PNETLAB Strore.          |
|   | - Giới hạn 10 tài khoản (Có thể nâng cấp). | 

## <a name ="1.3">1.3.  Ưu điểm</a>
  + Có phiển bản Offline.
  + Miễn phí
  + Hỗ trợ Lab Store, …
  + Hỗ trợ nhiều hệ điều hành (Cisco, Juniper, Arista, ..)
  + Hỗ trợ làm lab (Task, timer, …)
  + Không giới hạn Node.
  + Quản lý được dung lượng Ram, Cpu, Hdd cho từng thiết bị.
  + Hỗ trợ Wireshark, telnet, hot connections, Nat cloud, …

# <a name ="2">2.  Cài đặt PnetLab trên VMWare</a>
	
B1: Dowload tệp .ova tại link [trang chủ:](https://pnetlab.com/pages/download)

![image](https://user-images.githubusercontent.com/59860781/137439174-a75d863b-3acf-4fb5-8914-434f0a76193b.png)

B2: Triển khai trên các nền tảng ảo hóa như VirtualBox, VMWare, …

![image](https://user-images.githubusercontent.com/59860781/137439194-71967248-f0cd-4140-b528-f2d0f2983c7d.png)

B3: Đăng nhập:
- Sau khi cài đặt và thiết lập các cấu hình cơ bản. Đăng nhập vào pnetlab với tài khoản mặc định  username “root” password “pnet”.

![image](https://user-images.githubusercontent.com/59860781/137439212-c1df8e8b-a533-4f92-a258-6e9b8dce7485.png)

- Cài đặt mật khẩu cho tài khoản “root”

![image](https://user-images.githubusercontent.com/59860781/137439261-41752932-a201-462c-ab8f-71389fa532df.png)

![image](https://user-images.githubusercontent.com/59860781/137439266-7e6d1410-631b-490b-9ced-9befb8d86780.png)

- Đặt tên cho Pnet

![image](https://user-images.githubusercontent.com/59860781/137439279-abb98f63-994e-41b3-9050-340601c2cc3d.png)

- Cấu hình DNS domain name

![image](https://user-images.githubusercontent.com/59860781/137439305-1f6217ac-3fa4-4ea7-8913-b324798005d2.png)

- Cấu hình địa chỉ ip của PNETLab, có thể để DHCP hoặc Static

![image](https://user-images.githubusercontent.com/59860781/137439326-e4f5e9e7-e63d-4eb0-a2ee-404e26eaa9ca.png)

- Cấu hình máy chủ đồng bộ thời gian cho PNETLab

![image](https://user-images.githubusercontent.com/59860781/137439342-a13e51f5-523c-42e5-b951-92c7c842eb70.png)

- Cấu hình Proxy cho PNETLab

![image](https://user-images.githubusercontent.com/59860781/137439383-b0d23281-b920-47ed-86dc-d03c9b6f29ad.png)

- Tiến hành đăng nhập vào trang web với địa chỉ http://192.168.17.138

![image](https://user-images.githubusercontent.com/59860781/137439390-bb5b54f9-54ca-43ae-a115-78b89e347110.png)

- Có 2 tùy chọn đăng nhập: Chế độ trực tuyến và ngoại tuyến. Ở đây chúng ta sử dụng chế độ ngoại tuyến để sử dụng.  Sử dụng tài khoản mặc định: admin/pnet.

![image](https://user-images.githubusercontent.com/59860781/137439407-d45b33fc-7ab5-4114-96c5-043ac023419d.png)

- Sau khi đăng nhập ta có thể tạo các lab để tiến hành cấu hình.

![image](https://user-images.githubusercontent.com/59860781/137439423-8deb8ad2-1897-4cf7-9578-589380a2a468.png)

B4: Tải Lab từ cửa hàng:

- Truy cập vào PnetLab Store bằng [địa chỉ sau:](https://user.pnetlab.com/store/labs/view)

![image](https://user-images.githubusercontent.com/59860781/137439493-260ffcda-3505-4b50-ad5b-b51561a46718.png)

Note: Có rất nhiều Lab từ Store và các lab hoàn toàn miễn phí.

B5: Tải Lab và thực hành:
- Từ PNetLab Store, chọn một lab để thực hành (Ví dụ: VLANs Trungking and Routing on Cisco).

![image](https://user-images.githubusercontent.com/59860781/137439521-8a08c214-1fe1-42e9-bafa-00091360aa6a.png)

- Nhấn nút Dowload Lab sau đó điền địa chỉ IP và tiến hành Dowload

![image](https://user-images.githubusercontent.com/59860781/137439533-917d7041-1ea3-4f0c-8b6d-f7b2105955ce.png)

- Sau khi tải xong, ta quay trở lại PNetLab sẽ thấy Folder “Your labs from PNETLab Store”.

![image](https://user-images.githubusercontent.com/59860781/137439548-f35f8a2b-c7e6-4152-bcc4-a0f8c38bed44.png)

- Truy cập Folder “Your labs from PNETLab Store”

![image](https://user-images.githubusercontent.com/59860781/137439568-f6d4a76d-cd64-4330-b63e-8f9eecb410a5.png)

- Chọn vào Lab cần thực hành sau đó Open để tiến hành cấu hình.

![image](https://user-images.githubusercontent.com/59860781/137439591-3701a92b-4fa6-49b6-80d0-34867c6d110d.png)








