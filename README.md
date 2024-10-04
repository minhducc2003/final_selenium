# Chuẩn bị

- **Intellij**
- **Java** (java –version jdk-21_linux-x64_bin)
- **Chrome** version 114

# Cách cài đặt

- **CÀI ĐẶT**
  - Link source code: https://github.com/minhducc2003/final_selenium/tree/master
  - Chrome version 114.0.5735.110
    - Ubuntu: https://bestim.org/download.html?dlm-dp-dl=13218
    - Windows: https://bestim.org/download.html?dlm-dp-dl=13216
  - Java 21 (java 17 mình chưa thử)
    - Ubuntu: https://download.oracle.com/java/21/latest/jdk-21_linux-x64_bin.tar.gz
    - Windows: https://download.oracle.com/java/21/latest/jdk-21_windows-x64_bin.exe
  > Sau khi cài đặt, kiểm tra phiên bản Java bằng lệnh `java -version`
  - Intellij có nhiều phiên bản, hiện tại mình đang dùng bản 2023.2: https://www.jetbrains.com/idea/download/other.html

  - **CHẠY CODE**
    - Mở source code bằng Intellij
    - Mở `pom.xml` và thực hiện Load Maven changes bằng `ctrl + shift + O` hoặc click vào icon nhỏ ở góc màn hình trên bên phải (warning các bạn bỏ qua nhé, còn đỏ mới là vấn đề :) )

<div align="center">
  <img src="https://github.com/user-attachments/assets/01142e97-0e9a-461d-bbb2-de1fec6e6ace" alt="image">
</div>
    - Tìm file RunTestSuite.xml trong source tiến hành chạy - run( hoặc ctrl + shift + F10)

    
  - Config
<div align="center">
  <img src="https://github.com/user-attachments/assets/f3265fb9-6cef-4fe4-b964-85cfccad7116" alt="image">
</div>

- **KẾT QUẢ CHẠY**
  - Mình thử chạy testcases.DangNhap.DangNhapWebBanHang sẽ gồm 7 testcase( có thể check trong file `/test/java/testcases/DangNhapWebBanHang`
  - Chương trình sẽ tự động mở Chrome và truy cập vào trang web Maybi.com -> Đăng nhập -> Tự động điền tài khoản mật khẩu và tự động đăng xuất

![Screenshot from 2024-10-04 14-36-24](https://github.com/user-attachments/assets/f4f804b0-9127-4f0c-95f7-5a81b60d18ca)
    
![Screenshot from 2024-10-04 14-36-28](https://github.com/user-attachments/assets/dc8da366-40db-4ab6-81d7-f8d02b0f27eb)
- Chạy thành công sẽ pass 7/7 testcases
![Screenshot from 2024-10-04 14-43-23](https://github.com/user-attachments/assets/d999bf59-fc8f-4b7e-9f25-c889fd863870)
- Trong quá trình chạy sẽ gặp lỗi mình nghĩ là do trang web chặn spam
![Screenshot from 2024-10-04 14-42-26](https://github.com/user-attachments/assets/421ede12-3362-46b3-a967-c94dea2a8f5d)
   - Cách xử lý, có thể run lại các testcases fall để thử lại hoặc
   - Tăng `Thread.sleep` trong `/test/java/pages/DangNhapPage/`
     
![Screenshot from 2024-10-04 14-46-52](https://github.com/user-attachments/assets/443384ad-6b0c-49b7-89ce-cfce49f976e8)


