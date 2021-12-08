# PART: JAVASCRIPT

## PROBLEM

## QUESTION

1.  Có những loại func nào trong js?

    - **Declaration func** (dùng từ khóa function), **expression func** (dùng để gán, truyền tham số, không cần tên), **arrow func** (một cách viết ngắn gọn không cần tên func)
    - Expression func không được **hoisting** (không thể gọi nếu chưa định nghĩa)

2.  Có những cách nào để tạo object trong js?

    - **Object constructor** vs **Prototype**
    - Prototype bổ sung các thuộc tính và phương thức cho Object

3.  Có thể thay đổi độ dài của mảng js mà số lượng phần tử vẫn không đổi?

    - Thay đổi độ dài mảng bằng cách gán **length**
    - Kiến thức: **empty element of array**

4.  **PreventDefault** và **StopPropagation** khác gì nhau?

    - PreventDefault ngăn chặn các sự kiện khi có sự kiện xảy ra
    - StopPropagation ngăn chặn các sự kiện với các phần tử có liên quan (cùng phạm vi element, element cha)

5.  **Event listener** có 2 phương thức **addeventlistener** và **removeeventlistener** vậy nếu thêm nhiều event cho 1 element thì nó có hoạt động đồng thời không?

6.  Làm thế nào để **encode** và **decode** json trong javascript

    - **Stringify** để encode và **parse** để decode

7.  **Promise** là gì? **Sync** và **Async** khác gì nhau?

    - Js la ngôn ngữ đồng bộ(sync) nhưng lại có các phương thức bất đồng bộ(async) như **settimeout**, **setinterval**, **fetch**, **xmlhttprequest**, **read/write file**, …
    - Promise giúp xử lý vấn đề **callback hell** khi xử lý các function async
    - Promise có **2 phương thức** quan trọng là **resolve** (thành công), **reject** (thất bại)
    - Promise có **3 trạng thái** chính là **pending** (đang chờ kết quả, nó sẽ bị rò rỉ trạng thái nếu không được resolve hoặc reject), **fulfilled** (hoàn thành), **reject** (đã thất bại)
    - **Chain** trong promise sẽ giúp code gọn hơn nhưng không xử lý hoàn toàn được việc **callback hell**/**promise hell**
    - **Promise.resolve()** sẽ luôn trả về resolve, **Promise.reject()** sẽ luôn trả về reject, **Promise.all()** sẽ hợp nhất các promise

8.  Làm sao để biết 1 func async trong js khi nào hoàn thành

    - Sử dụng **callback func**

9.  **Async** và **Await** là gì?

    - **Async** - khai báo (async function someName(){...})
      - Tự động chuyển một function thành một Promise()
      - Các chức năng Async cho phép sử dụng await.
    - **Await** - tạm dừng thực thi các chức năng không đồng bộ (var result = await someAsyncCall();)
      - Await chỉ được hoạt động và sử dụng khi có khai báo Async.
      - Await nó chỉ hoạt động với Promise chứ không hoạt động với function có callback

10. ES6, ES7 là gì?

    - Viết tắt của **ECMAScript** (phiên bản thứ 6) và (phiên bản thứ 7)
    - Bao gồm các tính năng mới như:
      1. Block - Scoped Constructs Let and Cont
      2. Arrow Function
      3. Rest Parameter
      4. Destructuring Assignment in ES6
      5. Default Parameters in ES6
      6. Template Literals in ES6
      7. Multi-line String in ES6
      8. Enhanced Object Literals in ES6
      9. Promises in ES6
      10. Classes in ES6

11. So sánh **var**, **const**, **let** (**scope, hoisting, assignment**)
    - Giống: đều để khai báo biến
    - Khác: var là **globally scoped**, nếu trong **block** thì nó là **function/locally scoped**. var **có hỗ trợ hoisting**
      - **hoisting**: nghĩa là dù khai báo ở đâu thì biến đều sẽ được đem lên đầu scope trước khi code được thực hiện
      - **let** là **block scoped**, const và let thì không hỗ trợ hoisting
      - Với hoisting **var khởi tạo là undefined**, **let, const không có bất kỳ giá trị khởi tạo nên sinh ra lỗi Reference Error**
      - **const** là **block scope**, nếu kiểu của biến là **primitive (bao gồm string, number, boolean, null, và undefined)** **không thể tái khai báo hay cập nhật giá trị**. biến là **reference (bao gồm object, array, và function)** thì **có thể thay đổi giá trị cho thuộc tính của biến**

## NOTE
