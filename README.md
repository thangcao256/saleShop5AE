# saleShop5AE - Ứng dụng đặt, bán hàng đơn giản
Đây là ứng dụng Mobile mình viết - phục vụ cho đồ án môn Lập trình trên thiết bị di động
Công cụ, Ngôn ngữ sử dụng:
* Java
* PHP, REST API, WebService
* MySQL

## Chức năng đăng nhập
Màn hình giao diện thiết kế tối giản, dễ nhìn và không rối mắt. Bao gồm một số diểm như edit text nhập Email, edit text nhập mật khẩu, nút đăng nhập và text view đăng ký.
Đối với nhưng người dùng đã có tài khoản, thì chỉ cần nhập email và mật khẩu sau đó bấm nút đăng nhập. Ngay lúc đó hệ thống sẽ kiểm tra email đã tồn tại trong cơ sở dữ liệu hay chưa rồi tới kiểm tra mật khẩu. Nếu chính xác hệ thống sẽ điều hướng người dùng tới màn hình giao diện trang chủ. Nếu không chính xác thì hệ thống sẽ hiển thị thông báo tùy thuộc vào những dữ liệu người dùng truyền vào 2 trường này. Và nếu người dùng chưa có tài khoản thì có thể chọn vào mục đăng ký ngay.

    
![tripsviet](https://i.ibb.co/Sw0ftc0/1.png)

## Chức năng đăng ký
Màn hình giao diện thiết kế tối giản, dễ nhìn và không rối mắt. Bao gồm một số diểm như edit text nhập họ tên, edit text nhập Email, edit text nhập mật khẩu, edit text nhập lại mật khẩu và nút đăng ký.
Đây là phần giúp người dùng tạo một tài khoản để có thể thực hiện các chức năng nâng cao, người dùng cần nhập đầy đủ thông tin được yêu cầu, trong đó mật khẩu và nhập lại mật khẩu đã được mã hóa MD5 và phải trùng khớp với nhau. Sau cừng khi bấm nút đăng ký, hệ thống sẽ thêm tài khoản của người dùng vào cơ sở dữ liệu và xuất thông báo đăng ký thành công. Giờ đây người dùng có thể đăng nhập và sử dụng ứng dụng một cách bình thường.

![tripsviet](https://i.ibb.co/m6BKhns/2.png)

## Giao diện trang chủ
Màn hình giao diện trang chủ được sắp xếp theo bố cục hợp lý và hiện đại, Màn hình trang chủ như là một menu điều hướng người dùng tới tất cả những chức năng mà người dùng muốn thực hiện như: tìm kiếm, xem danh sách sản phẩm, xem giỏ hàng, chỉnh sửa thông tin cá nhân,… 

    
![tripsviet](https://i.ibb.co/ysqg3J9/3.png)

## Chức năng tìm kiếm
Chức năng tìm kiếm được tích hợp ngay phía trên cùng của màn hình giao diện, để sử dụng chức năng tìm kiếm, người dùng chỉ cần nhập vào thông tin của sản phẩm muốn tìm và chọn tìm kiếm. Ngay lập tức, hệ thống sẽ trả về kết quả của sản phẩm người dùng muốn tìm và cả những sản phẩm có chứa từ khóa do người dùng nhập vào.

    
![tripsviet](https://i.ibb.co/BjsDWss/15.png)

## Giao diện danh sách sản phẩm
Giao diện danh sách sản phẩm là item thứ 3 trong bottom menu ở trang chủ và đồng thời cũng được tích hợp ở màn hình trang chủ. Danh sách sản phẩm trả về tất cả những sản phẩm có trong cơ sở dữ liệu và chỉ hiện những sản phẩm còn hàng trong cơ sở dữ liệu.

    
![tripsviet](https://i.ibb.co/kyFBk6h/5.png)

## Giao diện chi tiết sản phẩm.
Mỗi sản phẩm đều có những thông tin thuộc tính khác nhau vì vậy để người dùng có cái nhìn tiệm cận nhất tới tất cả sản phẩm, thì người dùng chỉ cần bấm vào từng sản phẩm có trong danh sách sản phẩm. Với hệ thống được thiết kế kĩ lưỡng thì việc sản phẩm trả về đầy đủ và khớp vào những trường dữ liệu đã được thiết kế trước có mức độ chính xác gần như tuyệt đối. Trong chi tiết sản phẩm bao gồm thông tin chi tiết của sản phẩm kèm thoa nút thêm sản phẩm vào giỏ hàng và trở về danh sách sản phẩm

    
![tripsviet](https://i.ibb.co/H74Kx4b/6.png)

## Giao diện giỏ hàng
Phần lớn chức năng trong giỏ hàng đều ứng với từng sản phẩm, có thể kế đến như: tăng, giảm số lượng và xóa khỏi giỏ hàng. Mỗi khi người dùng bấm vào nút tăng(+) hoặc giảm(-) thì tổng tiền sản phẩm và tổng tiền giỏ hàng đều thay đổi tùy theo số lượng sản phẩm với công thức đã được quy định sẵn. Ngoài ra, còn có 1 số chức năng như mua hàng, trở về màn hình trang chủ và trở về danh sách sản phẩm.

    
![tripsviet](https://i.ibb.co/s1nt7hG/7.png)

## Giao diện đặt hàng.
Màn hình giao diện đặt hàng, là màn hình kết thúc chuỗi quá trình mua hàng của người dùng. Tại đây người dùng bắt buộc phải nhập những thông tin liên hệ cũng như địa chỉ để đội ngũ giao hàng có thể thực hiện giao hàng tới tay người dùng. Sau khi điền đúng và đủ thông tin thì người dùng cần bấm vào nút đặt mua, sau một khoảng thời gian thì nhân viên của hệ thống sẽ gọi điện để xác nhận đơn hàng của người dùng. Ngoài ra còn có nút hủy bỏ nếu người dùng cảm thấy không thích sản phẩm cũng như cháy túi.

    
![tripsviet](https://i.ibb.co/GMWqLQP/8.png)

## Giao diện thông tin người dùng
Màn hình giao diện người dùng là nơi thể hiện thông tin của người dùng. Tạo đây, người dùng có thể chỉnh sửa thông tin tùy ý muốn, ngoài ra còn có chức năng đăng xuất tài khoản. Vì đây là tài khoản của quản trị viên nên được mở rộng thêm chức năng quản lý sản phẩm.

    
![tripsviet](https://i.ibb.co/GMWqLQP/8.png)

## Giao diện quản trị viên
Quản trị viên của ứng dụng được cấp quyên để có thể thực hiện bộ chức năng CRUD(thêm, xóa, sửa) trên các đối tượng mà phần mềm quản lý. ở đây là quản lý điện thoại và quản lý hãng sản xuất.

    
![tripsviet](https://i.ibb.co/6DyDvwS/10.png)

## Giao diên ̣quản lý danh sách sản phẩm
Màn hình giao diện quản lý sản phẩm của quản trị viên khá tương đồng với màn hình hiển thị danh sách sản phẩm của phía người dùng. Nhưng đã được mở rộng thêm chức năng thêm sản phẩm.

    
![tripsviet](https://i.ibb.co/1zT6HQQ/11.png)

## Chức năng thêm sản phẩm.
Màn hình giao diện quản lý sản phẩm của quản trị viên khá tương đồng với màn hình hiển thị danh sách sản phẩm của phía người dùng. Nhưng đã được mở rộng thêm chức năng thêm sản phẩm.

    
![tripsviet](https://i.ibb.co/XzSZ8rT/12.png)

## Chức năng quản lý hãng sản xuất sản phầm
Màn hình giao diện danh sách hãng sản xuất được hệ thống trả về trong dữ liệu gồm những hãng sản xuất có sản phẩm trong dữ liệu. tại đây quản trị viên có thể theo dõi và có thể quản lý hãng sản xuất với bộ chức năng CRUD..

    
![tripsviet](https://i.ibb.co/6J2kCJX/13.png)

## Chức năng quản lý thêm loại sản phẩm.
Màn hình giao diện thêm thêm loại sản phẩm chỉ gồm 1 trưỡng dữ liệu là tên hãng sản xuất và một nút thêm mói. Khi người quản trị nhập thông tin hãng sản xuất thì bấm thêm mới. Hệ thống sẽ thêm hãng sản xuất vừa mới nhập vào hệ thống.

    
![tripsviet](https://i.ibb.co/F0M9gNv/14.png)

Link video demo: https://www.youtube.com/watch?v=j_QFPbusNDE

# saleShop5AE - Ứng dụng đặt, bán hàng đơn giản


    
    
    



    
