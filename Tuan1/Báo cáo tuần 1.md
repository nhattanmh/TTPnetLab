# MỤC LỤC
&ensp;[1, Khái niệm](#1)

&ensp;[1.1, VLAN](#1.1)

&ensp;[1.2,TRUNKING](#1.2)

&ensp;[2, Thực hành:](#2)

&ensp;[2.1. VLANs Trunking and Routing on Cisco](#2.1)

&ensp;[2.2. Configuration the VLANs on Switch Cisco](#2.2)

# <a name ="1">1.  Khái niệm:</a>
# <a name ="1.1">1.1.  VLAN:</a>
-	VLAN (Virtual LAN) là một hay nhiều LAN ảo được chia ra từ một Switch vật lý có tính chất tương tự như một switch vật lý. Nói cách khác VLAN là chia một switch vật lý thành nhiều switch logic độc lập.
VD: Để các host cùng VLAN của 2 switch có thể giao tiếp được nhau. 2 VLAN này phải được kết nối với nhau.
-	Dãy giá trị VLAN ID chạy từ 0 – 4095.
 - 1-1001: dải VLAN thường được sử dụng.
 - 1002 – 1005 : dải này dùng để giao tiếp với các kiểu mạng LAN khác.
 - 1006 – 4094: dải VLAN mở rộng, sử dụng khi switch hoạt động ở mode Transparent.
 - 0 và 4095: VLAN dành riêng.
 - VLAN 1, 1002 – 1005: mặc định trên Switch và không thể xóa được.Mặc định VLAN sau khi được tạo sẻ được lưu vào file vlan.dat trong bộ nhớ Flash.
