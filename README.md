# **Người Xoa Dịu** 
## _Ân Ngờ_ 
## Giới thiệu sơ qua MV ca nhạc :
NGƯỜI XOA DỊU | Ân ngờ X Boum [OFFICIAL MV] [From Mini Album 💿 0 Ngờ]  
Sáng tác: Ân ngờ, Boum  
Singer: Ân ngờ, Boum  
Link MV chính thức :  
https://youtu.be/m0WRscOG9oU?si=iPMHe_N6TRicxOs0  
Poster MV[^1] :  

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/b7e20afb-d182-406e-81e7-683118d744eb" />




Đây là một demo nhỏ và đơn giản về cách hiển thị các ảnh lên màn hình LCD_128x64 chạy liền mạch , nói đúng hơn là tạo gift 😅 .
Để làm được demo này , cần chuẩn bị vài thứ :
# 1 . Phần cứng :
+ Mạch vi xử lý Arduino Uno R3
+ Màn hình Graphic-LCD-128x64-ST7920
+ Dây cáp truyền dữ liệu cho Arduino
+ Các dây kết nối (Male & female Jumpings)
+ Breadboard
  
# 2 . Phần mềm :
+ Arduino IDE (version 2.3.+)
+ Tool Convert Image_to_byte_array[^2]
+ Code tham khảo trong REPO (intro_Nguoixoadiu_LCD.ino)
+ Images   
# Thực hành :
  Bắt tay vào làm thôi 🚀  
  Sơ đồ đấu nối dây (Source : Sưu tầm trên Internet):  
  
<img width="2064" height="1500" alt="LCD-SPI-ST7920-128x64" src="https://github.com/user-attachments/assets/d7f95dd4-284c-4860-a17e-605309c7d4b3" />


** ⚠️ Lưu ý:
__Tính toán dung lượng thực tế của Arduino Uno R3__ :  
Kích thước 1 ảnh (128x64): (128 × 64) / 8 = 1024 bytes (đúng bằng 1 KB).
Bộ nhớ Flash của Uno R3: Có tổng cộng 32 KB. Tuy nhiên, bootloader hệ thống đã chiếm mất 0.5 KB, nên bạn chỉ còn 31.5 KB trống cho toàn bộ code.  
Dung lượng của thư viện và code nền: Bản thân thư viện U8g2 khi khởi tạo cấu hình Full Buffer (_F_HW_SPI) cùng với các hàm đồ họa cơ bản sẽ tiêu 
tốn khoảng 5 KB đến 6 KB Flash.

_Lời khuyên_: Chỉ nên dùng dưới 20 images hoặc giải pháp thay thế là dùng các VXL khác mạnh hơn về bộ nhớ , tốc dộ xử lý như ESP32, Arduino Mega,..  
hoặc dùng module thẻ nhớ SD( Này tự tìm hiểu thêm :) ).

[^1]: https://i.ytimg.com/vi/m0WRscOG9oU/maxresdefault.jpg
[^2]: [image2cpp. ](https://javl.github.io/image2cpp/) 

_**Đây là sản phẩm demo nhằm mục đích giải trí , không liên quan gì đến chỉnh sửa nội dung của bài hát **_
