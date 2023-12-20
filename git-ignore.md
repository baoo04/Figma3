<!-- #Gitignore -->

1. Định nghĩa:
- gitignore là một tệp tin cấu hình trong hệ thống quản lý mã nguồn Git, được sử dụng để xác định những tệp và thư mục mà Git nên bỏ qua trong quá trình theo dõi sự thay đổi. Mục đích của nó là giảm dung lượng kho lưu trữ, tăng tốc quá trình đồng bộ hóa và giữ cho lịch sử phiên bản của dự án trở nên sạch sẽ và dễ đọc.

2. Cách thức hoạt động:
- Khi Git thực hiện theo dõi các thay đổi, nó sẽ kiểm tra tệp .gitignore trong thư mục làm việc hiện tại và các thư mục cha.
- Mỗi dòng trong tệp .gitignore đại diện cho một quy tắc để bỏ qua các tệp và thư mục cụ thể.
- Quy tắc có thể là tên tệp, mẫu thông tin đường dẫn, hoặc biểu thức chính quy, ....
- Dấu thanh gạch ngược "/" được sử dụng để chỉ định một thư mục cụ thể.
- Dấu * được sử dụng để bỏ qua mọi tệp và thư mục.
- Dấu ! trước quy tắc được sử dụng để loại trừ những tệp hoặc thư mục được định nghĩa trước đó.

3. Cú pháp:
- *.log: Bỏ qua tất cả các tệp có phần mở rộng là .log.
- build/: Bỏ qua thư mục có tên "build".
- /node_modules/: Bỏ qua thư mục node_modules, ngay cả khi nó không ở trong thư mục gốc.
- !important.log: Bao gồm tệp important.log mặc dù có một quy tắc bỏ qua tất cả các tệp .log.
- Sử dụng gitignore là một phần quan trọng của quá trình quản lý phiên bản và đảm bảo rằng chỉ những dữ liệu quan trọng và cần thiết nhất được theo dõi trong kho lưu trữ Git.
