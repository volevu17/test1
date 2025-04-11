# TẠO VPS STORAGE VỚI DỊCH VỤ CLOUD

Kính chào quý khách,

Sau khi quý khách đăng ký và thanh toán thành công, hệ thống sẽ tự động khởi tạo dịch vụ Cloud VPS và quý khách đã có thể tiến hành tạo máy chủ để sử dụng.

Các bước hướng dẫn bên dưới được thực hiện sau khi quý khách đã đăng nhập thành công vào trang Portal để quản lý dịch vụ (https://clients.vndata.vn/ ), sau khi đăng nhập thành công thì thực hiện theo các bước sau:

### Bước 1: THÊM MÁY CHỦ MỚI 
- Quý khách click vào **Thêm máy chủ mới** 1 trong 2 chỗ như trên hình.
![1](https://github.com/volevu17/test1/blob/main/%E1%BA%A3nh%201.png?raw=true)

- Đối với quý khách đã có 1 hoặc nhiều máy chủ trước thì sẽ chọn **Thêm máy chủ mới bên tay trái**, vì tab bên tay phải sẽ hiển thị máy chủ hiện có:

 ![2](https://github.com/volevu17/test1/blob/main/%E1%BA%A2nh2.png?raw=true)

### Bước 2: GIAO DIỆN "TẠO MÁY CHỦ MỚI"

 ![3](https://github.com/volevu17/test1/blob/main/3.png?raw=true)

- **Tên máy chủ**: Là hostname (đối với Linux), Computer name (đối với Windows).
- **Mật khẩu**: quý khách sẽ sử dụng mật khẩu này để kết nối đến máy chủ, ssh (đối với Linux), remote desktop (đối với Windows).
- **SSH Keys (nếu có)**: hoặc quý khách có thể bỏ qua bước này nếu không muốn sử dụng public ssh key: chỉ hoạt động đối với OS Linux, quý khách có thể add public ssh key của máy mình lên server thông qua quá trình khởi tạo.
  - Để add ssh key vào server, quý khách click chuột vào Quản lý SSH Keys.
  - Trang web sẽ chuyển sang phần add ssh key.
  - Quý khách chọn “ Add new ssh key “.


### Bước 3: LỰA CHỌN HỆ ĐIỀU HÀNH 
- Quý khách chọn từ danh sách hệ điều hành có sẳn. Chúng tôi sẽ liên tục cập nhật các hệ điều hành phổ biến và mới nhất có thể ở danh sách này.

 ![4](https://github.com/volevu17/test1/blob/main/4.png?raw=true)


### Bước 4: CHỌN CẤU HÌNH MÁY ẢO 

-  Mặc đinh hệ thống sẽ tự động mặc định thông số tối đa của gói toàn bộ tài nguyên của quý khách, quý khách có thể tùy chỉnh để phân chia số lượng máy chủ của mình mong muốn nếu cần tạo nhiều máy ảo hơn:

 ![5](https://github.com/volevu17/test1/blob/main/5.png?raw=true)

### Bước 5: KHỞI TẠO MÁY ẢO 
- Sau khi bấm nút **Tạo máy ảo mới** thì máy chủ của quý khách đang khởi tạo, quý khách vui lòng chờ đến khi máy chủ khởi tạo hoàn tất. Thời gian tạo mới đối với máy ảo chạy hệ điều hành Windows Server (30 phút) sẽ lâu hơn Linux (5 phút).

- Quá trình khởi tạo tất, trang web sẽ tự động chuyển sang trang mới với tất cả thông tin máy chủ quý khách.

 ![6](https://github.com/volevu17/test1/blob/main/6.png?raw=true)

 Đến đây máy chủ ảo của quý khách đã tạo xong, quý khách có thể truy cập vào để sử dụng.

 - **Đối với máy chủ ảo thuộc nhóm Linux**: quý khách có thể kết nối qua giao thức SSH với port mặc định là 22 và username mặc định là vmadmin (đây là user thuộc group sudo).
 - **Đối với máy chủ thuộc nhóm Windows Server**: quý khách có thể kết nối qua giao thức RDP với port mặc định là 3389.



---

# ADD THÊM DISK HDD VÀO VPS STORAGE

Kính chào quý khách,

Sau đây sẽ là hướng dẫn các bước thao tác để add thêm disk HDD vào máy chủ ảo Cloud VPS. Quý khách vui lòng thực hiện theo các bước sau.

### Bước 1: CHỌN MÁY ẢO CẦN NÂNG CẤP

- Chọn máy ảo cần nâng cấp và tắt máy (shutdown) để đảm bảo an toàn. Quý khách có thể shutdown trực tiếp từ bên trong máy chủ hoặc bấm nút **Tắt nguồn**.

   ![7](https://github.com/volevu17/test1/blob/main/7.png?raw=true)


### Bước 2: NÂNG CẤP Ổ CỨNG (STORAGE) CỦA MÁY CHỦ ẢO

- Sau khi shutdown bấm vào mục Storage

 ![8](https://github.com/volevu17/test1/blob/main/8.png?raw=true)

 - **Add new disk**: Gắn thêm 1 disk mới vào máy chủ ảo. Quý khách có thể mount ổ đĩa mới này lên 1 phân vùng mới để lưu dữ liệu, hoặc join ổ đĩa này vào volume group hiện có trên máy chủ (nếu có cấu hình trước đó)

 - Mặc đinh hệ thống sẽ tự động mặc định thông số tối đa của gói toàn bộ tài nguyên của quý khách, quý khách có thể tùy chỉnh để phân chia số lượng máy chủ của mình mong muốn nếu cần tạo nhiều máy ảo hơn:


 ![9](https://github.com/volevu17/test1/blob/main/9.png?raw=true)

 ### Bước 2: TIẾN HÀNH KHỞI ĐỘNG LẠI MÁY CHỦ VÀ KIỂM TRA KẾT QUẢ

 ![10](https://github.com/volevu17/test1/blob/main/10.png?raw=true)

- Bài viết trên đây là toàn bộ hướng dẫn thực hiện việc nâng cấp ổ đĩa HDD của máy chủ ảo, nếu quý khách gặp khó khăn trong quá trình thực hiện vui lòng liên hệ bộ phận hỗ trợ kỹ thuật để được hỗ trợ nhanh chóng.
 ---
 # MOUNT DISK HDD TRÊN OS LINUX VÀ WINDOWS

   ### 1. MOUNT DISK TRÊN UBUNTU
 
### 1.1. Kiểm tra phân vùng.

- Để kiểm tra ổ đĩa đã được phân vùng chưa thì chúng ta dùng lệnh như sau: lsblk

   ![11](https://github.com/volevu17/test1/blob/main/11.png?raw=true)

### 1.2. Phân vùng ổ đĩa.

 - Nếu ổ đĩa chưa được phân vùng, hãy sử dụng lệnh: fdisk
 - Trong fdisk:
  - Gõ *n* để tạo phân vùng mới
  - Gõ *p* để Primary
  - Chọn số (mặc định là 1)
  - Nhấn **Enter** vài lần để chấp nhận mặc định
  - Gõ *w* để ghi lại và thoát

   ![13](https://github.com/volevu17/test1/blob/main/13.png?raw=true)

- Sau khi tạo phân vùng thành công hãy kiểm tra bằng lênh: lsblk

 ![14](https://github.com/volevu17/test1/blob/main/14.png?raw=true)

- Quý khách sẽ thấy /dev/sbd1


### 1.3. Tạo filesystem cho phân vùng 

- Xóa toàn bộ dữ liệu trên phân vùng bằng lệnh: sudo mkfs.ext4

![15](https://github.com/volevu17/test1/blob/main/15.png?raw=true)

### 1.4. Tạo thư mục để mount và mount lại 

 - Để tạo một thư mục để mount, chúng ta dùng lệnh: sudo mkdir /mnt/*Tên thư mục*

 - Tiếp theo mount ổ đĩa đã được phân vùng vào thư mục vừa tạo ra bằng lệnh: sudo mount /dev/sdb1 /mnt/*Tên thư mục*

   ![16](https://github.com/volevu17/test1/blob/main/16.png?raw=true)

### 1.5. Kiểm tra mount

- Để kiểm tra ổ đĩa đã được mount, quý khách dùng lệnh *df -hT*, quý khách sẽ thấy /mnt/*Tên thư mục* được mount với loại filesystem là *ext4*

 ![17](https://github.com/volevu17/test1/blob/main/17.png?raw=true)


### 2. MOUNT DISK TRÊN WINDOWS

- **Bước 1:** Chạy **Run** và nhập dòng lệnh **diskmgmt.msc** để vào được *Disk Management*

![18](https://github.com/volevu17/test1/blob/main/18.png?raw=true)

- **Bước 2:** Sau khi vào được *Disk Management*, quý khách sẽ thấy được một ổ đĩa đã được thêm vào là **Disk 1**
  
![19](https://github.com/volevu17/test1/blob/main/19.png?raw=true)

- **Bước 3:** Click chuột phải vào **Disk 1** chọn *Online* để bật **Disk 1**
  ![20](https://github.com/volevu17/test1/blob/main/20.png?raw=true)

- **Bước 4:** Click chuột phải vào vùng màu đen => chọn **New Simple Volume**

  ![21](https://github.com/volevu17/test1/blob/main/21.png?raw=true)

- **Bước 5:** Sau khi chọn **New Simple Volume** sẽ mở một hộp thoại mới, Để chọn dung lượng

   ![22](https://github.com/volevu17/test1/blob/main/22png.png?raw=true)

- **Bước 6:** Chọn *Next* để tiếp tục và gán ký tự ổ đĩa (ví dụ: *E:* )

 ![23](https://github.com/volevu17/test1/blob/main/23.png?raw=true)

- **Bước 7:** Chọn *Next* để qua một hộp thoại mới và chọn hệ thống tập tin tùy vào nhu cầu của quý khách

 ![24](https://github.com/volevu17/test1/blob/main/24.png?raw=true)

- **Bước 8:** Sau khi Mount thành công ta vào **This PC** để xem xuất hiện một ổ đĩa mới

 ![26](https://github.com/volevu17/test1/blob/main/26.png?raw=true)
  
- Trong bài viết này mình đã hướng dẫn Mount ổ đĩa HDD thêm vào máy chủ trên 2 hệ điều hành đang thông dụng và phổ biến hiện nay. Chúc các bạn thao tác và thực hiện thành công.












 







