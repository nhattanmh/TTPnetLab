# MỤC LỤC
&ensp;[1. Khái niệm](#1)

&ensp;[1.1. VLAN](#1.1)

&ensp;[1.2. TRUNKING](#1.2)

&ensp;[2. Thực hành:](#2)

&ensp;[2.1. VLANs Trunking and Routing on Cisco](#2.1)

&ensp;[2.2. Configuration the VLANs on Switch Cisco](#2.2)

# <a name ="1">1.  Khái niệm:</a>
# <a name ="1.1">1.1.  VLAN:</a>
-	VLAN (Virtual LAN) là một hay nhiều LAN ảo được chia ra từ một Switch vật lý có tính chất tương tự như một switch vật lý. Nói cách khác VLAN là chia một switch vật lý thành nhiều switch logic độc lập.
VD: Để các host cùng VLAN của 2 switch có thể giao tiếp được nhau. 2 VLAN này phải được kết nối với nhau.
- Dãy giá trị VLAN ID chạy từ 0 – 4095.
   -  1-1001: dải VLAN thường được sử dụng.
   -  1002 – 1005 : dải này dùng để giao tiếp với các kiểu mạng LAN khác.
   -  1006 – 4094: dải VLAN mở rộng, sử dụng khi switch hoạt động ở mode Transparent.
   -  0 và 4095: VLAN dành riêng.
   -  VLAN 1, 1002 – 1005: mặc định trên Switch và không thể xóa được.Mặc định VLAN sau khi được tạo sẻ được lưu vào file vlan.dat trong bộ nhớ Flash.

# <a name ="1.2">1.2.  TRUNKING:</a>
Đường trunk được dùng để kết nối hoặc đấu nối giữa các Switch
- Các chuẩn Trunking trong hệ thống mạng:
   -  Chuẩn IEEE và kỹ thuật trunking DOT1Q..
   -  Native VLAN trong kỹ thuật Trunking.
   -  Chuẩn Cisco và kỹ thuật trunking ISL.
VD: Các host cùng một VLANs trên 2 hoặc nhiều thiết bị muốn đi đến nhau thì giữa các Switch này phải có một hoặc nhiều đường đấu nối (Trunk) với nhau. Giả sử hệ thống bạn có quá nhiều VLAN. Giữa các VLAN trên các Switch có quá nhiều đường đấu nối là không hợp lý. Nên cần có một giải pháp chỉ cần một đường kết nối mà vẫn đảm bảo tính thông suốt của các VLAN. 
- Lúc này Switch chỉ cần dành ra một đường kết nối để thông suốt các VLAN trên các Switch lại với nhau.

# <a name ="2">2.  Thực hành:</a>

# <a name ="2.1">2.1.  VLANs Trunking and Routing on Cisco</a>
# Mô hình

![image](https://user-images.githubusercontent.com/59860781/137440703-bc6eebd7-14c2-4ba1-96c9-a95adbb64df9.png)

Yêu cầu: Thiết lập cấu hình VLANs Trungking and Routing để các thiết bị thuộc sự quản lý của Switch A có thể ping thông tới thiết bị thuộc sự quản lý của Switch B.

- Truy cập vào Switch A.
- Tiến hành tạo vlan và đặt tên cho vlan.

![image](https://user-images.githubusercontent.com/59860781/137440741-05346860-9a4d-49f2-a9d1-0d3d3bab2a0b.png)

- Tiến hành xác đinh port mà thiết bị cần access VLAN tiến hành cấu hình VLAN cho port đó.

![image](https://user-images.githubusercontent.com/59860781/137440758-28f9479b-77c5-4422-92cc-b6e301758cdf.png)

- Kiểm tra Vlan vừa tạo.

![image](https://user-images.githubusercontent.com/59860781/137440777-d96848c8-e620-4682-b158-c4a5d838edfa.png)

- Tiến hành cấu hình Trunking cho đường đi giữa 2 Switch.

![image](https://user-images.githubusercontent.com/59860781/137440798-f51d5559-cd52-4ac8-8c06-1db3cb350955.png)

- Truy cập vào Switch B.
- Tiến hành tạo vlan và đặt tên cho vlan.

![image](https://user-images.githubusercontent.com/59860781/137440810-1ee04b93-5b88-4392-9b8a-c3017b2e74b6.png)

- Tiến hành xác đinh port mà thiết bị cần access VLAN tiến hành cấu hình VLAN cho port đó.

![image](https://user-images.githubusercontent.com/59860781/137440831-6e8b1020-2ffa-4a65-be37-7b78c4de3986.png)

- Kiểm tra Vlan vừa tạo.

![image](https://user-images.githubusercontent.com/59860781/137440838-a3b27860-0292-4998-8e4f-739b898d9ca7.png)

- Tiến hành cấu hình Trunking cho đường đi giữa 2 Switch.

![image](https://user-images.githubusercontent.com/59860781/137440854-37de2945-79b7-463e-9794-10fb7158cc07.png)

- Truy cập vào thiết bị Sistermas 1 (192.168.1.1) tiến hành ping tới thiết bị Sistermas 4 (192.168.1.4), để kiểm tra kết nối.

![image](https://user-images.githubusercontent.com/59860781/137440861-1cbd3309-d80a-4c5f-9691-f17cf9fb2711.png)

# <a name ="2.2">2.2.  Configuration the VLANs on Switch Cisco</a>
# Mô hình

![image](https://user-images.githubusercontent.com/59860781/137440928-c0103022-9bf8-4298-8b83-98c1316b3833.png)

- Truy cập vào Switch A.
- Tiến hành tạo vlan và đặt tên cho vlan.

![image](https://user-images.githubusercontent.com/59860781/137440950-06b3b9f9-be8b-46ba-bf3b-95189c9c7d6a.png)

- Tiến hành xác đinh port mà thiết bị cần access VLAN tiến hành cấu hình VLAN cho port đó.

![image](https://user-images.githubusercontent.com/59860781/137440968-8d864561-0d8e-4d50-aee7-479113391683.png)

- Kiểm tra Vlan vừa tạo.

![image](https://user-images.githubusercontent.com/59860781/137440994-c24c113c-bf3e-43fa-978e-d63f1d50b569.png)

- Tiến hành cấu hình Trunking cho đường đi giữa 2 Switch.

![image](https://user-images.githubusercontent.com/59860781/137441004-df0612e4-aa1f-4256-8a17-a281deb4406c.png)

- Kiểm tra cấu hình của Switch

![image](https://user-images.githubusercontent.com/59860781/137441008-6e25cc0c-9d35-4c9c-a698-586bcf482f7f.png)

![image](https://user-images.githubusercontent.com/59860781/137441013-338e8839-ad34-48b1-922b-c8a346816781.png)

- Truy cập vào Switch B.
- Tiến hành tạo vlan và đặt tên cho vlan.

![image](https://user-images.githubusercontent.com/59860781/137441029-5749ba9f-523c-4576-8f09-2ebd848559a4.png)

- Tiến hành xác đinh port mà thiết bị cần access VLAN tiến hành cấu hình VLAN cho port đó.

![image](https://user-images.githubusercontent.com/59860781/137441035-4db85789-5366-43a4-99e9-53821bededf3.png)

- Kiểm tra Vlan vừa tạo. 

![image](https://user-images.githubusercontent.com/59860781/137441043-a022eeca-5192-4e56-b797-e22edd7f187b.png)

- Tiến hành cấu hình Trunking cho đường đi giữa 2 Switch.

![image](https://user-images.githubusercontent.com/59860781/137441053-90416ce3-8999-4cc1-8210-4dbc7554a9a8.png)

- Kiểm tra cấu hình của Switch

![image](https://user-images.githubusercontent.com/59860781/137441066-98f3ad1b-c7bf-437d-8281-969313aef055.png)

![image](https://user-images.githubusercontent.com/59860781/137441071-8e69ae3a-4de9-4a90-a102-2a10f2c052fb.png)

- Truy cập vào thiết bị Sistermas 1 (192.168.1.1) tiến hành ping tới thiết bị Sistermas 4 (192.168.1.4), để kiểm tra kết nối.

![image](https://user-images.githubusercontent.com/59860781/137441089-0e39dbbe-6bcf-4972-9762-e017a1f43a20.png)




