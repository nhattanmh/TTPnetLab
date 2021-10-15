# MỤC LỤC
&ensp;[1, Tìm hiểu về PNET LAB](#1)

&ensp;[1.1,	Giới thiệu](#1.1)

&ensp;[1.2.	Mode PNETLAB](#1.2)

&ensp;[1.3.	Ưu điểm](#1.3) 

&ensp;[2.	Cài đặt PnetLab trên VMWare](#2)


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

# <a name ="2>2.  Cài đặt PnetLab trên VMWare</a>
	
B1: Dowload tệp .ova tại link [trang chủ:](https://pnetlab.com/pages/download)
