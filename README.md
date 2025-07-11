# đọc file txt trên laptop khác.
#cai node 12.18.3
    https://nodejs.org/dist/v12.18.3/
# Cài đặt nvm:
    https://github.com/coreybutler/nvm-windows/releases
# edit Dòng đầu tiên của code:
    const fs = require('node:fs');
    Sửa thành:
    const fs = require('fs');
# Kiểm tra phiên bản hiện tại của chokidar:
    npm list chokidar
# Nếu không thấy, có thể bạn chưa cài đặt nó trong thư mục dự án. Gỡ phiên bản hiện tại (nếu có):
    npm uninstall chokidar
# Cài đặt phiên bản 3.3.1:
    npm install chokidar@3.3.1
# npm init // enter tới kết thúc.
    npm install
    node app.js
#Ctrl + c // end
# form chu
    CMD: chcp 65001 // UTF-8
    cd C:/Users/NMXLNT3/Desktop/sync_folder
# Cài pm2 toàn cục:
    npm install -g pm2
    Chạy app.js với pm2: pm2 start app.js
    Kiểm tra trạng thái:pm2 list
    Xem log: pm2 logs
    Dừng nếu cần:
    pm2 stop app.js
    pm2 stop 0
    Dùng id: pm2 delete 0
    Dùng name: pm2 delete app
# pm2 start app.js --name sync_folder_to_edmsoft
# start to window
    npm install pm2-windows-startup -g
    pm2-start install
    pm2 start app.js
    pm2 save
