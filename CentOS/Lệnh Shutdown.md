Lệnh shutdown có nhiều tiện ích mà đôi khi chúng ta không biết hoặc không biết hết công dụng của nó. Thông thường để shutdown máy hay reboot máy tính chúng ta thường dùng lệnh init 0 hoặc init 6, nhưng sau đây tôi sẽ chỉ bạn một số cách shutdown và hẹn lịch shutdown máy như sau (Để sử dụng lệnh shutdown bạn cần phải có quyền root.

1. Để reboot máy ngay lập tức bạn dùng lệnh sau:

`shutdown -r now`

2. Giả sử bạn cần chạy một cái gì đó và sau đó cần shutdown máy bạn dùng lệnh sau:
Lệnh này nói cho hệ thống biết sau 10 phút nữa hãy shutdown máy tính.
Lệnh này có thể dùng cho việc reboot máy bằng cách thay -h bằng -r
shutdown -h +10
3. Nếu bạn muốn shutdown máy sau một số giây nhất định thì bạn dùng lệnh sau:
Lệnh này nói cho hệ thống biết sau 3 giây nữa hãy kill các process và shutdown máy.
shutdown -t3 -r now
4. Giả sử bạn là người hay thích nghe nhạc trước khi đi ngủ hoặc bạn hay ngủ quên mà không tắt máy tính thì lệnh sau sẽ rất hữu ích cho bạn – tôi thường dùng lệnh này :
Lệnh này nói cho hệ thống biết lúc 1 giờ đêm (nếu dùng +24h) hãy shutdown máy.
Tương tự ta có thể thay -h bằng -r để reboot máy.
shutdown -h 01:00
