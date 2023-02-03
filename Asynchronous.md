## Xử lý bất đồng bộ trong javascript, NodeJS

### Callback
- Trước đây thường xử dụng callback để xử lý bất đồng bộ trong js

### Promise
- một instance promise được khởi tạo từ new Promise();
- bên trong constructor new Promise() sẽ nhận đối số truyền vào là 1 callback, trong callback này có 2 param là resolve và reject
- Tùy vào xử lý bên trong callback mà ta sẽ gọi hàm resolve() (thành công) hay reject() (thất bại)
- Các xử lý trong callback của new Promise() sẽ chạy trước khi instance promise.then().catch().finall()
- Nếu thành công (callback trả về resolve) thì hàm .then() sẽ được gọi
- Nếu thất bại (callback trả về reject) thì hàm .catch() sẽ được gọi
- .finally() sẽ luôn được gọi
### Async/Await
- Async/Await được xây dựng trên Promises
- `Async` được khai báo ở đầu method, thông báo đây là hàm bất đồng bộ
- Nếu khai báo `Async` Tự động biến đổi một hàm thông thường thành một Promise.
- `Async` cho phép sử dụng `Await`.
- `Await` sẽ tạm dừng việc thực hiện các hàm async
- Khi từ `await` được đặt trước 1 promise, thì nó sẽ đợi cho promise đó thực hiện xong và trả về kết quả
- Await chỉ làm việc với Promises
- Await chỉ có thể được sử dụng bên trong các function async.
