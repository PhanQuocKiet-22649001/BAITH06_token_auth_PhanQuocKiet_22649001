1. Profile

Method = GET
URL: http://localhost:3000/api/auth/profile
-Quyền truy cập bị từ chối vì chưa có tài khoản và đăng nhập
<img width="1919" height="1079" alt="image" src="public/img/failprofile.png" />

2. Register

Method = POST
URL: http://localhost:3000/api/auth/register

- đăng ky thành công với thông tin 
{
"username": "admin",
"email": "admin@gmail.com",
"password": "123"
}
<img width="1919" height="1079" alt="image" src="public/img/register.png" />
-Tài khoản được lưu trong database
<img width="1919" height="1079" alt="image" src="public/img/registerdb.png" />

3. Login
Method = POST
URL: http://localhost:3000/api/auth/login

-TH đăng nhập thất bại sẽ trả về thông báo " "error": "Invalid credentials""
<img width="1919" height="1079" alt="image" src="public/img/faillogin.png" />

-TH đăng nhập thành công, sẽ trả về token có giá trị: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY4ZDdlNDc5OTIxNDY5NTU2ODI2ZjE2ZSIsImlhdCI6MTc1ODk3OTQwNywiZXhwIjoxNzU4OTgzMDA3fQ.1P8dVsKfoQkyI2vcCves9i_XBixsnYO1zEFXsAtXlpI"

<img width="1919" height="1079" alt="image" src="public/img/login.png" />

4. Truy cập trang Profile sau khi login thành công
- Copy token được postman trả về ở bước login
- Chọn qua tab Authozization, chọn Bearer Token
- Dán token đã copy vào
- đã truy cập thành công và trả về thông tin của tài khoản
<img width="1919" height="1079" alt="image" src="public/img/profile.png" />



