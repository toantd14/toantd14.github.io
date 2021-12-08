# PART: JAVASCRIPT

## QUESTION

1.  Có những loại func nào trong js?
    - **Declaration func** (dùng từ khóa function), **expression func** (dùng để gán, truyền tham số, không cần tên), **arrow func** (một cách viết ngắn gọn không cần tên func)
    - Expression func không được **hoisting** (không thể gọi nếu chưa định nghĩa),...

2.  Có những cách nào để tạo object trong js?
    - **Object constructor** vs **Prototype**
    - Prototype bổ sung các thuộc tính và phương thức cho Object
    - Có thể tạo object bằng từ khoá **new** và xoá bằng từ khoá **delete**

3.  Có thể thay đổi độ dài của mảng js mà số lượng phần tử vẫn không đổi?
    - Thay đổi độ dài mảng bằng cách gán **length**
    - Kiến thức: **empty element of array**

4.  **Truthy** và **Falsy** là gì?
    - Bất cứ giá trị nào trong Javascript khi chuyển đổi sang kiểu dữ liệu boolean mà có giá trị true thì ta gọi giá trị đó là **Truthy**.
    - Ngược lại có giá trị false thì ta gọi giá trị đó là **Falsy**.

5.  **PreventDefault** và **StopPropagation** khác gì nhau?
    - PreventDefault ngăn chặn các sự kiện khi có sự kiện xảy ra
    - StopPropagation ngăn chặn các sự kiện với các phần tử có liên quan (cùng phạm vi element, element cha)

6.  **Event listener** có 2 phương thức **addeventlistener** và **removeeventlistener** vậy nếu thêm nhiều event cho 1 element thì nó có hoạt động đồng thời không?

7.  Làm thế nào để **encode** và **decode** json trong javascript
    - **Stringify** để encode và **parse** để decode

8.  Phân biệt **đơn luồng** và **đơn luồng bất đồng bộ**
    - Js là ngôn ngữ đồng bộ(sync) nhưng lại có các phương thức bất đồng bộ(async) như **settimeout**, **setinterval**, **fetch**, **xmlhttprequest**, **read/write file**, …
    - Đơn luồng đồng bộ: Code xử lý từng dòng từ trên xuống dưới, nếu gặp yêu cầu tốn thời gian -> dừng toàn bộ và chờ phản hồi
    - Đơn luồng bất đồng bộ: Xử lý theo thời gian kết thúc, Thứ tự sắp xếp dựng vào
      - Ưu tiên macro task (browser Api như: setTimeout, event) hay micro task (promise)
      - Dùng callback, promise để bắt output và sắp xếp thứ tự kết quả theo mong muốn

9.  **Promise** là gì? **Sync** và **Async** khác gì nhau?
    - Promise giúp xử lý vấn đề **callback hell** khi xử lý các function async
    - Promise có **2 phương thức** quan trọng là **resolve** (thành công), **reject** (thất bại)
    - Promise có **3 trạng thái** chính là **pending** (đang chờ kết quả, nó sẽ bị rò rỉ trạng thái nếu không được resolve hoặc reject), **fulfilled** (hoàn thành), **reject** (đã thất bại)
    - **Chain** trong promise sẽ giúp code gọn hơn nhưng không xử lý hoàn toàn được việc **callback hell**/**promise hell**
    - **Promise.resolve()** sẽ luôn trả về resolve, **Promise.reject()** sẽ luôn trả về reject, **Promise.all()** sẽ hợp nhất các promise

10. Làm sao để biết 1 func async trong js khi nào hoàn thành
    - Sử dụng **callback func**

11. **Async** và **Await** là gì?
    - **Async** - khai báo (async function someName(){...})
      - Tự động chuyển một function thành một Promise()
      - Các chức năng Async cho phép sử dụng await.
    - **Await** - tạm dừng thực thi các chức năng không đồng bộ (var result = await someAsyncCall();)
      - Await chỉ được hoạt động và sử dụng khi có khai báo Async.
      - Await nó chỉ hoạt động với Promise chứ không hoạt động với function có callback

12. So sánh callback, promise, async/await

13. ES6, ES7 là gì?
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

14. So sánh **var**, **const**, **let** (**scope, hoisting, assignment**)
    - Giống: đều để khai báo biến
    - Khác: var là **globally scoped**, nếu trong **block** thì nó là **function/locally scoped**. var **có hỗ trợ hoisting**
      - **hoisting**: nghĩa là dù khai báo ở đâu thì biến đều sẽ được đem lên đầu scope trước khi code được thực hiện
      - **let** là **block scoped**, const và let thì không hỗ trợ hoisting
      - Với hoisting **var khởi tạo là undefined**, **let, const không có bất kỳ giá trị khởi tạo nên sinh ra lỗi Reference Error**
      - **const** là **block scope**, nếu kiểu của biến là **primitive (bao gồm string, number, boolean, null, và undefined)** **không thể tái khai báo hay cập nhật giá trị**. biến là **reference (bao gồm object, array, và function)** thì **có thể thay đổi giá trị cho thuộc tính của biến**

15. Arrow func có những đặc điểm gì khác với declare func, express func?
    - Arrow func sử dụng toán tử => để tạo func, nếu muốn trả về object mà không dùng clock code thì thêm dấu () bao lại object
    - Arrow func không có this (biến context)
    - Arrow func không thể dùng để làm constructor func

16. Phân biệt toán tử **Rest** và **Spread**
    - Giống: cùng dùng dấu **...** để để khai báo
    - Rest dùng để lấy ra các phần tử còn lại trong 1 mảng (...<tên-biến>) - được áp dụng khi sử dụng **Destructuring**
    - Spread được sử dụng để hợp nhất mảng hoặc object

17. **import** và **export** trong es6
    - tương tự như cách **include/require** 1 file trong php, nhằm mục đích sử dụng các variable, object, module từ 1 file khác

18. **Polyfill** là gì? Cách triển khai một Polyfill?
    - là định nghĩa 1 func thay thế cho func chưa được hỗ trợ bởi trình duyệt cũ

19. So sánh declaration func, expression func, arrow func, closure

20. So sánh hiệu năng giữa việc sử dụng closures và prototype


## REFERENCE
- [The Modern JavaScript Tutorial](https://javascript.info/)
- [Complete JavaScript](https://completejavascript.com/javascript/)
- [JavaScript MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [ECMAScript 6 — New Features: Overview & Comparison](http://es6-features.org/)
- [JavaScript Cơ Bản F8 Edu](https://fullstack.edu.vn/courses/javascript-co-ban)
- [JavaScript Nâng Cao F8 Edu](https://fullstack.edu.vn/learning/javascript-nang-cao)
- [Hoisting trong JavaScript](https://viblo.asia/p/hoisting-trong-javascript-Eb85oaM4Z2G)

## KEY NOTE

1. Key Note 1
   1. Length
   2. Find index
   3. Cut string
   4. Replace
   5. Convert to upper case
   6. Convert to lower case
   7. Trim
   8. Split
   9. Get a character by index

2. Key Note 2
   1. Event Listener
   2. JSON
   3. Promise
   4. Fetch
   5. DOM Location
   6. Local Storage
   7. Session Storage
   8. Coding Convention
   9. Best Practice
   10. Mistakes
   11. Performance

3. Key Note 3
   1. var, let, const
   2. Template literals
   3. Multi-line string
   4. Arrow function
   5. Classes
   6. Default parameter values
   7. Destructuring
   8. Rest parameters
   9. Spread
   10. Enchanced object literals
   11. Tagged template literal
   12. Modules
   13. Optional chaining (?.)

4. Key Note 4
   1. IIFE
   2. Clusures
   3. Hoisting
   4. Strict mode
   5. This keyword
   6. Bind keyword
   7. Call method
   8. Apply method
   9. Catching, throwing, errors
   10. Promise
   11. Async func, await func


