# I. TẠO VPS STORAGE VỚI DỊCH VỤ CLOUD

Kính chào quý khách,

Sau khi quý khách đăng ký và thanh toán thành công, hệ thống sẽ tự động khởi tạo dịch vụ Cloud VPS và quý khách đã có thể tiến hành tạo máy chủ để sử dụng.

Các bước hướng dẫn bên dưới được thực hiện sau khi quý khách đã đăng nhập thành công vào trang Portal để quản lý dịch vụ (https://clients.vndata.vn/ ), sau khi đăng nhập thành công thì thực hiện theo các bước sau:

### Bước 1: THÊM MÁY CHỦ MỚI 
- Quý khách click vào **Thêm máy chủ mới**.

<div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/001.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Đối với quý khách đã có 1 hoặc nhiều máy chủ trước thì sẽ chọn **Thêm máy chủ mới bên tay trái**

### Bước 2: GIAO DIỆN "TẠO MÁY CHỦ MỚI"

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/002.png?raw=true" alt="Demo Image" width="800"/>
</div>

 

- **Tên máy chủ**: Là hostname (đối với Linux), Computer name (đối với Windows).
- **Mật khẩu**: quý khách sẽ sử dụng mật khẩu này để kết nối đến máy chủ, ssh (đối với Linux), remote desktop (đối với Windows).
- **SSH Keys (tùy chọn)**: hoặc quý khách có thể bỏ qua bước này nếu không muốn sử dụng public ssh key: chỉ hoạt động đối với OS Linux, quý khách có thể add public ssh key của máy mình lên server thông qua quá trình khởi tạo.
  - Để add ssh key vào server, quý khách click chuột vào Quản lý SSH Keys.
  - Trang web sẽ chuyển sang phần add ssh key.
  - Quý khách chọn “ Add new ssh key “.


### Bước 3: LỰA CHỌN HỆ ĐIỀU HÀNH VÀ CẤU HÌNH MÁY ẢO
- Quý khách chọn từ danh sách hệ điều hành có sẳn. Chúng tôi sẽ liên tục cập nhật các hệ điều hành phổ biến và mới nhất có thể ở danh sách này.

  <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/003.png?raw=true" alt="Demo Image" width="800"/>
</div>



- Mặc định, hệ thống sẽ tự động phân bổ toàn bộ tài nguyên tối đa theo gói dịch vụ mà quý khách đã đăng ký. Tuy nhiên, quý khách hoàn toàn có thể tùy chỉnh lại các thông số để phù hợp với nhu cầu, đặc biệt khi muốn tạo nhiều máy chủ ảo từ cùng một gói.

 - Storage: Quý khách có 2 sự lựa chọn
   - OS Storage: Nơi cài đặt hệ điều hành
   - HDD Storage: Dành cho lưu trữ dữ liệu phụ, data, backup,...

### Bước 4: KHỞI TẠO MÁY ẢO 
- Sau khi bấm nút **Tạo máy ảo mới** thì máy chủ của quý khách đang khởi tạo, quý khách vui lòng chờ đến khi máy chủ khởi tạo hoàn tất. Thời gian tạo mới đối với máy ảo chạy hệ điều hành Windows Server (15 - 20 phút) sẽ lâu hơn Linux (5 phút).

- Quá trình khởi tạo tất, trang web sẽ tự động chuyển sang trang mới với tất cả thông tin máy chủ quý khách.

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/004.png?raw=true" alt="Demo Image" width="800"/>
</div>

 Đến đây máy chủ ảo của quý khách đã tạo xong, quý khách có thể truy cập vào để sử dụng.

 - **Đối với máy chủ ảo thuộc nhóm Linux**: quý khách có thể kết nối qua giao thức SSH với port mặc định là 22 và username mặc định là vmadmin (đây là user thuộc group sudo).
 - **Đối với máy chủ thuộc nhóm Windows Server**: quý khách có thể kết nối qua giao thức RDP với port mặc định là 3389.



---

# II. ADD THÊM DISK HDD VÀO VPS STORAGE

Kính chào quý khách,

Sau khi tạo thành công VPS Storage, quý khách tiền hành thêm disk HDD

### Bước 1: CHỌN MÁY ẢO CẦN NÂNG CẤP

- Chọn máy ảo cần nâng cấp và quý khách chọn tab "Storage" trong giao diện quản lý VPS.

   <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/005.png?raw=true" alt="Demo Image" width="800"/>
</div>


### Bước 2: NÂNG CẤP Ổ CỨNG (STORAGE) CỦA MÁY CHỦ ẢO


 - **Add new disk**: Gắn thêm 1 disk mới vào máy chủ ảo. Quý khách có thể mount ổ đĩa mới này lên 1 phân vùng mới để lưu dữ liệu, hoặc join ổ đĩa này vào volume group hiện có trên máy chủ (nếu có cấu hình trước đó)

 - Mặc đinh hệ thống sẽ tự động mặc định thông số tối đa của gói toàn bộ tài nguyên của quý khách, quý khách có thể tùy chỉnh để phân chia số lượng máy chủ của mình mong muốn nếu cần tạo nhiều máy ảo hơn:

  <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/006.png?raw=true" alt="Demo Image" width="800"/>
</div>

 ### Bước 3: TIẾN HÀNH KHỞI ĐỘNG LẠI MÁY CHỦ VÀ KIỂM TRA KẾT QUẢ

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/007.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Bài viết trên đây là toàn bộ hướng dẫn thực hiện việc nâng cấp ổ đĩa HDD của máy chủ ảo, nếu quý khách gặp khó khăn trong quá trình thực hiện vui lòng liên hệ bộ phận hỗ trợ kỹ thuật để được hỗ trợ nhanh chóng.
 ---
 # III. MOUNT DISK HDD BÊN TRONG OS LINUX VÀ WINDOWS

 Kính chào Quý khách,

 Sau khi đã thêm thành công ổ đĩa HDD vào máy chủ Cloud VPS, Quý khách vui lòng tiếp tục thực hiện các bước sau để mount ổ đĩa vào hệ điều hành và sử dụng cho mục đích lưu trữ dữ liệu.

   ### 1. MOUNT DISK TRÊN UBUNTU
 
### 1.1. Kiểm tra phân vùng.

- Để kiểm tra ổ đĩa đã được phân vùng chưa thì chúng ta dùng lệnh như sau: lsblk

    <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/008.png?raw=true" alt="Demo Image" width="800"/>
</div>

### 1.2. Tạo Partition.

 - Nếu ổ đĩa chưa được phân vùng, hãy sử dụng lệnh: fdisk
 - Trong fdisk:
  - Gõ *n* để tạo phân vùng mới
  - Gõ *p* để Primary
  - Đánh số thứ tự cho phân vùng (mặc định là 1)
  - Nhấn **Enter** vài lần để chấp nhận mặc định
  - Gõ *w* để ghi lại và thoát

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/009.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Sau khi tạo phân vùng thành công hãy kiểm tra bằng lênh: lsblk

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/010.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Quý khách sẽ thấy /dev/sdb1


### 1.3. Định dạng lại phân vùng ở trên

- Quý khách cần tạo hệ thống tập tin (chẳng hạn ext4) để phân vùng có thể sử dụng được trong hệ điều hành.

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/011.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Hệ thống tập tin EXT4 hỗ trợ: Kích thước tệp tối đa: 16TB
- Hệ thống tập tin EXT3 hỗ trợ: Kích thước tệp tối đa: 2TB
- Hệ thống tập tin EXF hỗ trợ: Kích thước tệp tối đa: 8EB
Và còn nhiều hệ thống tệp khác nữa, quý khách có thể lựa chọn tùy vào nhu cầu.

### 1.4. Mount Partition 

 - Ví dụ tạo một thư mục để mount, chúng ta dùng lệnh: sudo mkdir /mnt/*Tên thư mục*

 - Tiếp theo mount ổ đĩa đã được phân vùng vào thư mục vừa tạo ra bằng lệnh: sudo mount /dev/sdb1 /mnt/*Tên thư mục*

    <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/012.png?raw=true" alt="Demo Image" width="8000"/>
</div>

### 1.5. Kiểm tra

- Để kiểm tra ổ đĩa đã được mount, quý khách dùng lệnh *df -hT*, sẽ hiển thị danh sách các phân vùng đã được mount cùng với định dạng hệ thống tập tin.
  
  <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/013.png?raw=true" alt="Demo Image" width="800"/>
</div>

### 1.6. Tự động Mount sau khi Reboot
 - Lấy UUID của phân vùng
    <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/014.png?raw=true" alt="Demo Image" width="800"/>
</div>

- Mở file fstab để chỉnh sửa bằng lệnh: *sudo nano /etc/fstab*

  
 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/015.png?raw=true" alt="Demo Image" width="800"/>
</div>

- **UUID=....:** Định danh duy nhất của phân vùng
- **/mnt/data:** Điểm mount
- **ext4:** Loại hệ thống tập tin
- **0**: Không cần dump
- **2**: Kiểm tra lỗi sau root (root */* là *1*)



### 2. MOUNT DISK TRÊN WINDOWS

- **Bước 1:** Chạy **Run** và nhập dòng lệnh **diskmgmt.msc** để vào được *Disk Management*

- **Bước 2:** Sau khi vào được *Disk Management*, quý khách sẽ thấy được một ổ đĩa đã được thêm vào là **Disk 1**
  
 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/016.png?raw=true" alt="Demo Image" width="800"/>
</div>

- **Bước 3:** Click chuột phải vào **Disk 1** chọn *Online* để Online **Disk 1**
   <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/017.png?raw=true" alt="Demo Image" width="800"/>
</div>

- **Bước 4:** Click chuột phải vào **Unallocated** => chọn **New Simple Volume**

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/018.png?raw=true" alt="Demo Image" width="800"/>
</div>

- **Bước 5:** Sau khi chọn **New Simple Volume** sẽ mở một hộp thoại mới

- **Bước 6:** Chọn *Next* để tiếp tục và điều chỉnh kích thước ổ đĩa

   <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/019.png?raw=true" alt="Demo Image" width="800"/>
</div>

  - **Maximum disk space in MB:** Dung lượng tối đa mà bạn có thể gán cho phân vùng này (tính theo MB). Đây là dung lượng trống có sẵn trên ổ đĩa.
  - **Minimum disk space in MB:** Dung lượng tối thiểu mà bạn có thể gán (thường là 8MB trở lên).
  - **Simple volume size in MB:** Mặc định là dung lượng tối đa, nhưng bạn có thể chỉnh lại tùy ý. Đây là kích thước thực tế của phân vùng mới.


- **Bước 7:** Chọn *Next* để tiếp tục và gán ký tự ổ đĩa.

  <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/020.png?raw=true" alt="Demo Image" width="800"/>
</div>

  - **Assign the following drive letter:** Tùy chọn gán ký tự ổ đĩa cho phân vùng này (ở đây là E:). 
  - **Mount in the dollowing empty NTFS folder:** Nếu chọn, quý khách có thể gắn phân vùng vào một thư mục trống trên ổ đĩa NTFS khác thay vì gán ký tự ổ đĩa.
  - **Do not assign a drive letter or drive path:** Không gán ký tự hay đường dẫn nào, phân vùng sẽ không hiển thị trong **File Explorer**.

  - Trong bài hướng dẫn này, quý khách lựa chọn **Assign the following drive letter** 

- **Bước 8:** Chọn *Next* để qua một hộp thoại mới và chọn hệ thống tập tin tùy vào nhu cầu của quý khách

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/021.png?raw=true" alt="Demo Image" width="800"/>
</div>

 - **Do not format this volume:** Không định dạng. Nếu chọn mục này, bạn phải format sau khi tạo xong nếu muốn sử dụng được.
 - **Format this volume with the following settings:** Trong quá trình phân vùng có thể định dạng cùng lúc.
    - **File system:** Lựa chọn hệ thống tệp tin theo nhu cầu của quý khách.
    - **Allocation unit size:** Kích thước đơn vị phân bổ.
    - **Volume label:** Tên hiển thị của ổ đĩa này trong File Explorer.
    - **Perform a quick format:** Định dạng nhanh, không kiểm tra bad sector. Nếu bỏ chọn thì sẽ format kỹ hơn (mất thời gian hơn).
    - **Enable file and folder compression:** Nén tệp và thư mục trong ổ đĩa này để tiết kiệm không gian

 - Trong bài hướng dẫn này, quý khách lựa chọn **Format this volume with the following settings** và đặt tên cho Volume.
   
    - **Bước 9:** Kiểm tra Mount

 <div align="center">
  <img src="https://github.com/volevu17/test1/blob/main/022.png?raw=true" alt="Demo Image" width="800"/>
</div>
  
- Trong bài viết này mình đã hướng dẫn Mount ổ đĩa HDD thêm vào máy chủ trên 2 hệ điều hành đang thông dụng và phổ biến hiện nay. Chúc quý khách thao tác và thực hiện thành công.












 







