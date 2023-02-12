## git status: Hiển thị trạng thái
Câu lệnh này sẽ hiển thị:
 - Bạn đang ở branch nào
 - Trạng thái branch của bạn so với origin như thế nào (cái này nhiều lúc không chính xác vì dữ liệu đã được thay đổi trên origin, muốn chính xác thì phải `git fetch` để tải về dữ liệu mới nhất)
 - Trạng thái file trong dự án, file nào đang được git track (theo dõi)
## Các khu vực làm việc với git
Chúng ta sẽ có các khu vực theo thứ tự dưới đây

Khu vực làm việc: Chính là nơi chúng ta đang code, vẫn ở local
Khu vực staging: Sau khi dùng git add thì file sẽ được đưa lên khu vực này, vẫn ở trên local
Khu vực committed: Sau khi dùng git commit thì file từ staging sẽ được đưa lên đây, cũng vẫn ở trên local
Khu vực remote (gọi origin cũng được): Sau khi dùng git push sẽ file ở commited lên đây, bây giờ file của bạn đã đưa lên trên server
## git add: Thêm file vào khu vực staging
## git reset: Khôi phục những file ở khu vực Staging về khu vực code
## git commit: commit code
## git push: đẩy code lên git server
## git log: Hiển thị log commit (Hiển thị những thông tin commit gần nhất)
 - Nếu muốn nhìn những thông tin rút gọn: `git log --oneline`
## git pull: Kéo code từ remote pepo về
## Bỏ qua file với .gitignore
Cách viết `.gitignore`
 - Comment thì dùng `#`
 - Ignore file: abc.exe
 - Ignore thư mục: folder/
 - Phủ định thì thêm `!`
 - Ignore tất cả các file có đuôi là `.exe`: `*.exe`