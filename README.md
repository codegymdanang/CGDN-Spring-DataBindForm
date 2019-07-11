#CGDN-Spring-DataBindForm

Trong bài này chúng ta sử dụng Maven, Spring MVC, @RequestMapping,ModelAndView, Jstl để xây dựng chức năng quản lý sinh viên trên 1 trang website gồm có các chức năng:
1.	Hiển thị danh sách sinh viên: Lấy danh sách sinh viên từ class StudentServiceImpl sau đó dùng modelAndView trả dữ liệu về trang index.jsp và dùng thư viện jstl để hiển thị.

2.	Thêm 1 sinh viên mới: dùng method = GET trong RequestMapping của phương thức create() để trả về trang create.jsp, trên trang này có 1 form để nhập thông tin về sinh viên mới và method = post. Khi form này được submit, nó sẽ gửi dữ liệu sinh viên mới đến phương thức create() có RequestMapping method là POST, phương thức này sẽ xử lý lưu lại sinh viên và redirect lại trang home.

3.	Sửa thông tin 1 sinh viên: dùng method = GET trong RequestMapping của phương thức edit() để trả về trang edit.jsp với thông tin sinh viên lấy được theo id. trên trang này cũng có 1 form để nhập thông tin mới về sinh viên và method = post. Khi form này được submit, nó sẽ gửi dữ liệu mới của sinh viên đến phương thức edit() có RequestMapping method là POST, phương thức này sẽ xử lý lưu lại sinh viên và redirect lại trang home.


4.	Xoá 1 sinh viên: dùng method = GET trong RequestMapping của phương thức delete() để trả về trang delete.jsp với thông tin sinh viên lấy được theo id. trên trang này cũng có 1 form để hiển thị thông tin về sinh viên bị xoá và method = post. Khi form này được submit, nó sẽ gửi dữ liệu của sinh viên bị xoá đến phương thức delete() có RequestMapping method là POST, phương thức này sẽ xử lý xoá sinh viên đó và redirect lại trang home.

