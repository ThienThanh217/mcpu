**********************************************************************************
*** Danh Sách Lệnh cài đặt tools xmrigcc miner để đào tất cả các coin chạy cpu ***
**********************************************************************************
*** CÁC LỆNH LINUX PHỤ TRỢ:

    rm -f [Tên File Cần Xóa]
    
    rm -r [Tên Thư Mục Cần Xóa]
    
    mrdir [Tên Thư Mục Cần Tạo]
    
    mv [Tên File Muốn Đổi] [Tên File Mới]

**********************************************************************************
0- LỆNH CẤP QUYỀN Admin

    sudo su

1- TẬP LỆNH UPDATE HỆ THỐNG:

    apt-get update -y 
    apt-get upgrade -y
    apt-get install wget 
    apt-get install get 
    apt-get install nano
    apt-get install git -y

2- Tải và cài đặt ứng dụng xmrigcc để khai thác coin:

    git clone https://github.com/ThienThanh217/mcpu.git
    cd mcpu
    tar xvaf xmrigcc-miner-arm-android-3.4.6.tar.gz
    chmod u+x xmrigDaemon
    chmod u+x xmrigMiner
    chmod +x config.json

3- Chỉnh sửa tập tin " config.json "  trước khi khai thác:

--cc-disabled : Vô hiệu hóa tính năng CC Client
--algo=ALGO : Gán thuật toán cần đào
--coin=COIN : Gán tên coin cần đào
--url=URL : Gán địa chỉ và cổng pools hồ khai thác coin
--user=USERNAME : Gán địa chỉ ví để tra coin khai thác về
--pass=PASSWORD : Gán mật khẩu của pools hồ khai thác nếu có, mặc định không có sẽ là "x"
--rig-id=ID : Gán tên thợ đào cho tứng máy nếu bạn có nhiều hơn 1 máy để tiền khai thác
--cpu-max-cpu-usage=N : Gán số cpu để khai thác (Theo %, ví dụ bạn có 8 cpu nhưng bạn chỉ muốn chạy 6 cpu thôi thì [N= 100* 6/8] (%) )

4- LỆNH KHAI THÁC COIN XMR:
Vui long tham khảo các file đào coin trong phần tệp thư mục
