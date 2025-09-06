**********************************************************************************
*** Danh Sách Lệnh cài đặt tools xmrigcc miner để đào tất cả các coin chạy cpu ***
**********************************************************************************
*** Các lệnh phụ trợ tham khảo:

    rm -f [Tên File Cần Xóa]
    
    rm -r [Tên Thư Mục Cần Xóa]
    
    mrdir [Tên Thư Mục Cần Tạo]
    
    mv [Tên File Muốn Đổi] [Tên File Mới]


**********************************************************************************
0- Lệnh Cấp Quyền Admin

    sudo su

1- Tập lệnh hệ thống update:

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

Máy 01:XMR_M01_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M01_S9pX --cpu-max-cpu-usage=80

Máy 02:XMR_M02_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M02_S9pH --cpu-max-cpu-usage=80

Máy 03:XMR_M03_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M03_S9pH --cpu-max-cpu-usage=80

Máy 04:XMR_M04_S9pX

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M04_S9pX --cpu-max-cpu-usage=80

Máy 05:XMR_M05_S9X

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M05_S9X --cpu-max-cpu-usage=80

Máy 06:XMR_M06_S10pT

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M06_S10pT --cpu-max-cpu-usage=80

Máy 07:XMR_M07_N8

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M07_N8 --cpu-max-cpu-usage=80

Máy 08:XMR_M08_S8pT

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M08_S8pT --cpu-max-cpu-usage=80

Máy 09:XMR_M09_A72017

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M09_A72017 --cpu-max-cpu-usage=80

Máy 10:XMR_M10_S9pH

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M10_S9pH --cpu-max-cpu-usage=80

Máy 11:uXMR_M11_M30s

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=uXMR_M11_M30s --cpu-max-cpu-usage=80

Máy 12:XMR_M12_G2plx

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M12_G2plx --cpu-max-cpu-usage=80

Máy 13:XMR_M13_SH701sh

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M13_SH701sh --cpu-max-cpu-usage=80

Máy 14:XMR_M14_ZFlip1

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=XMR --url=gulf.moneroocean.stream:10032 --user=869XzJgVi5tPtWiGHpFsYW9evJJzsUKZ2gmw1hiU75dGcwVEm6zTepJcCTTHaPYV79YX2BmQg7iTnQyvPdHzUeZr1nKWWGp --pass=x --rig-id=XMR_M14_ZFlip1 --cpu-max-cpu-usage=80

Máy 12:XMR_M12_G2plx

    ./xmrigDaemon --cc-disabled --algo=rx/0 --coin=SAL --url= sg.salvium.gfwroute.com:1230 --user=SaLvs7JKyBj5GhxwCZotD4GFeCkSWtLbB13ZZL6uExd28U4M6Z1DgW2AyP6LPYFGHtJyweuHASrg2Eei4GvakzvnVyodTxgSLHm --pass=x --rig-id=SAL_M11_M30s --cpu-max-cpu-usage=80
