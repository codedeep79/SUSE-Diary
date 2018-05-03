# SUSE-Diary
Some things collect about SUSE

+ SUSE Studio
+ VMware Cloud on AWS: Include all the enterprise tools you’re familiar with including vSphere, ESXi, VSAN and NSX
+ SUSE OpenStack Cloud
+ Hybrid Cloud with AWS
+ SoftNas Cloud
+ Hesive Cloud: Deploy .iso exist to GCP, Oracle, AWS; Build Lab Data center; Build visualization lab,...
+ VMware vSphere: VMWare vSphere là bộ sản phẩm của VMWare, dùng để phục vụ nhu cầu ảo hóa hệ thống. vSphere gồm 3 thành phần chính:
  + VMWare ESXi Server: Lớp ảo hóa chính chạy trên nền server vật lý ( hay còn gọi là Hypervisor ), có nhiệm vụ quản lý tài nguyên phần ứng và phân phát cho các máy ảo ( Virtual Machines )
  + VMware vCenter Server: Trung tâm quản lý chính của môi trường ảo hóa. Gồm các tính năng chính:
    + **vMotion**: Cho phép di chuyển các VM đang chạy từ 1 server vật lý này sang server vật lý khác mà k có downtime. Máy VM được chuyển sẽ hoạt động bình thường trong lúc di chuyển. Không thể dùng vMotion trong trường hợp chuyển VM từ DataCenter này sang DataCenter khác.
    + **Storage vMotion**: Cho phép di chuyển data virtual disk hoặc file cấu hình của VM từ DataStore này sang DataStore khác mà xảy ra gián đoạn dịch vụ.
    + **High Availability (HA)**: Tính năng giúp tăng tính sẵn sàng cho VM. Nếu Server chết, thì VM sẽ đc chuyển sang Server  phù hợp và start nó lên lại (có downtime)
    + **Fault Tolerance (FT)**: nâng cao tính sẵn sàng bằng cách tạo 1 bản sao của VM chính ( primary VM ) và chạy song song ( secondary VM ), và khi VM chính chết, VM phụ sẽ lập tức thay thế (không có downtime)
    + **Distributed Resource Scheduler (DRS)**: Phân phối và cân bằng các VM trên mỗi ESXi server, tránh tình trạng server thì quản lý quá nhiều VM, server khác thì chỉ quản lý vài VM.
    + **Distributed Power Management (DPM)**: Giảm năng lượng tiêu thụ.
    + **Storage DRS**: Giống DRS nhưng Storage DRS làm việc với các thiết bị lưu trữ, giúp cân bằng tài nguyễn gữa các DataStore.
  + VMWare vSphere Client: Chương trình cho phép truy cập, quản lý từ xa vào vCenter (hoặc ESXi ) – chỉ chạy trên Windows OS.
    + VMware vSphere Web Client: Chương trình trên web-browser cho phép truy cập từ xa vào vCenter – chạy trên mọi OS.
+ Ravello cloud


+ Install Java 8:

```
zypper install java-1_8_0-openjdk
zypper install java-1_8_0-openjdk-devel
update-alternatives --config java
update-alternatives --config javac
```

+ Install Git Server:

```
sudo zypper install git
```
