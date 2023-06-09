<h1>Tìm Hiểu Về Công Nghệ Front End and Back End</h1>
<h2>Mục Lục</h2>
<h3><a href="#Section1">I. Tìm hiểu Về ASP.Net
    </a></h3>
<ol>
    <li>
        <h3><a href="#Section11">Tìm hiểu về cấu trúc dự liệu trong ASP.Net</a></h3>
    </li>
    <li>
        <h3><a href="#Section12">Tìm hiểu về LinQ</a></h3>
    </li>
    <li>
        <h3><a href="#Section13">Tìm hiểu về Mô Hình MVVM</a></h3>
    </li>
</ol>
<h3><a href="#Section2">II. Tìm Hiểu Về Note.JS, Knockout.JS
    </a></h3>
<ol>
    <li>
        <h3><a href="#Section21">Cơ bản về Note JS</a></h3>
    </li>
    <li>
        <h3><a href="#Section22">Cơ bản về Knockout JS</a></h3>
    </li>
</ol>
<hr>
</hr>

<h3 id="user-content-section1" dir="auto">I. Tìm hiểu Về ASP.Net</h3>

<h4 id="user-content-section11" dir="auto">1. Tìm hiểu về cấu trúc dự liệu trong ASP.Net</h4>
<h4>File Startup cs</h4>
<p>
    Tại đây dùng để cấu hình các service cần thiết cho ứng dụng để xử lý các request.</br>
    VD: Bạn cũng có thể cấu hình sử dụng các loại dịch vụ (service) nào, như Dependency Injection, Logging.
    Và cũng cấu hình các dịch vụ cho đa môi trường.
</p>

<h4>File Program cs</h4>
<p>
    Tạo 1 web Server, hay web host.
    File này chứa class Program chịu trách nhiệm cấu hình nền tảng (infrastructure) của ứng dụng.
</p>
<p>Luồng chạy dữ liệu: Bắt đầu từ file Program.cs ==> Startup.cs ==> Sau khi khởi tạo các biến môi trường và hệ
    thống
    để chuẩn bị chạy, sau đó Chương trình sẽ chờ 1 hành động nào đó của user để tiếp tục xử lý.
</p>
<h4>Thư mục Connected Services:</h4>
<p> Connected Services sẽ làm việc khi chúng ta thêm 1 services bên ngoài vào ví dụ như: Cloud Storage with Azure
    Storage, …
</p>
<h4>Thư mục Dependencies:</h4>
<p>
    Dependencies
</p>
<h4>Thư mục Propeties:</h4>
<p>
    Propeties, tại thư mục này chứa file launchSetting.json, file này sẽ chứa các profile để chúng ta thực thi ứng
    dụng ( Chúng ta có thể thấy tại nút play run chương trình màu xanh lá cây như IIS Express => khi kéo xuống chúng
    ta sẽ thấy Profile ISS Express + Tên Chính của Thư mục Profile chính ). Và cũng có thể setup đa mội trường tại
    đây. Và file này chỉ chạy trên Local, còn khi lên Server chủ yếu sẽ chạy vào các môi trên file appsetting.
</p>

<pre>

    {
    "iisSettings": {
        "windowsAuthentication": false,
        "anonymousAuthentication": true,
        "iisExpress": {
    "applicationUrl": "http://localhost:8307",
        "sslPort": 0
        }
    },
    "profiles": {
        "IIS Express": {
        "commandName": "IISExpress", // IIS Express là cách chạy mặc định Visual Studio lựa chọn cho bạn
        "launchBrowser": true,
        "environmentVariables": {
            "ASPNETCORE_ENVIRONMENT": "Development"
        }
        },
        "xinchao": {
        "commandName": "Project",
        "launchBrowser": true,
        "environmentVariables": {
            "ASPNETCORE_ENVIRONMENT": "Development"
        },
        "dotnetRunMessages": "true",
        "applicationUrl": "http://localhost:5000"
        }
    }
    }   
</pre>

<h4>Thư mục wwwroot</h4>
<p>wwwroot là thư mục của ứng dụng, và tất cả như các file html, css, image, … đều đặt trong này.</p>

<h4>File: tên project.csproj</h4>
<p>Tại đây ta có thể thêm và quản các package hỗ trợ phát triển ứng dụng.</p>

<h4>File: libman.json</h4>
<p>Tại đây giúp chúng ta tải và sắp xếp thư mục của các thư viện hỗ trợ khi phát triển ứng dụng, như các thư viện
    của JS, ...
</p>

<h4 id="user-content-section12" dir="auto">2. Tìm hiểu về LinQ</h4>
<p>LINQ (Language Integrated Query) - ngôn ngữ truy vấn tích hợp - nó tích hợp cú pháp truy vấn ( gần giống các câu lệnh
    SQL ) dựa trên ngôn ngữ lập trình C#,
    cho nó có khả năng truy cập các nguồn dữ liệu khác nhau (SQL Db, XML, List ...) với cùng cú pháp.</p>
<pre>
    public class Product
    {
        public int ID {set; get;}
        public string Name {set; get;}         // tên
        public double Price {set; get;}        // giá
        public string[] Colors {set; get;}     // các màu sắc
        public int Brand {set; get;}           // ID Nhãn hiệu, hãng
        public Product(int id, string name, double price, string[] colors, int brand)
        {
            ID = id; Name = name; Price = price; Colors = colors; Brand = brand;
        }
        // Lấy chuỗi thông tin sản phẳm gồm ID, Name, Price
        override public string ToString()
           => $"{ID,3} {Name, 12} {Price, 5} {Brand, 2} {string.Join(",", Colors)}";
    
    }
</pre>

<a href="https://codelearn.io/sharing/linq-la-gi-va-no-hoat-dong-nhu-the-nao">Link tham khảo thêm</a>

<h4 id="user-content-section13" dir="auto">3. Tìm hiểu về Mô Hình MVVM</h4>

<p>MVVM không phải là framework hay thư viện, api…
    nó chỉ đơn thuần là hướng dẫn bạn định nghĩa cấu trúc ứng dụng của bạn.
    MVVM được phát triển dựa trên kiến trúc MVP.</p>
<p>
    Trong các mô hình truyền thống, chúng ta thường xử lý sự kiện Click và viết mã thực thi trực tiếp ở trên một Button
    nhưng với mô hình MVVM không cho phép làm điều này.
    Trong mô hình MVVM, các điều khiển(control) như Button, ListView, SearchBar, v.v.
    không thể kết buộc trực tiếp đến dữ liệu mà phải thông qua thuộc tính Command hay Controler.
</p>
<p>
    Trong thư mục Views chứ các file giao diện. Và mỗi file giao diện đều có class code-behind đi kèm.
    Đặc biệt file code-behind ta sẽ không sử dụng đến, mọi điều cần làm sẽ chuyển xuống class ViewModel.
</p>
<h4>Cấu trúc thư mục trong MVVM</h4>
<h4>- Views</h4>
<p>Trong thư mục Views chứ các file giao diện. Và mỗi file giao diện đều có class code-behind đi kèm.
    Đặc biệt file code-behind ta sẽ không sử dụng đến, mọi điều cần làm sẽ chuyển xuống class ViewModel.</p>
<h4>- Models</h4>
<p>Trong thư mục Models trong đó tạo các class chứa data và bất kỳ liên kết validation,
    logic nghiệp vụ để chắc chắc
    tính toàn vẹn của data,
    bạn có thể tách ra thư mục Repositories khác. Chúng được dùng như một phần của mô hình MVVM.</p>
<h4>- ViewModels</h4>
<p>ViewModels sẽ sử dụng các model liên kết giữa View-ViewModel giúp chúng gửi và nhận dữ liệu
    ( Binding,DataContext, Behaviors SDK ).
</p>

<h3 id="user-content-section2" dir="auto">II. Tìm Hiểu Về Note.JS, Knockout.JS</h3>
<h3 id="user-content-section21" dir="auto">1. Cơ Bản về Note JS</h3>
Note Js bản chất của nó là 1 cái vỏ bọc bên ngoài, nó giống 1 môi trường, nó không phải là 1 ngôn ngữ, không
phải là
Framework, là 1 môi trường giúp các bạn chạy được trên môi trường máy chủ bằng code javascript ( hỗ trợ từ C++
làm
nền tảng kết nối với máy chủ )
<h4>Kiến thức hỗ trợ để hiểu rõ hơn về Note JS</h4>
<h4>Client - Server</h4>
<p>
    Client có thể hiểu là giao diện nơi người dùng có thể gửi các request đến server.
</p>
<p>
    - VD Client là gì, như các giao diện duyệt web như Chrome, Firefox, .., hay gọi là giao diện dành cho
    người dùng.
</p>
<p>
    Server là nơi sẽ phản hồi yêu cầu từ Client bằng Notejs ( dựa trên ngôn ngữ javascipt ), gửi về VD gói tin
    như (
    html,csss, javascript, … )
</p>
<h4>NPM - chương trình quản lý thư viện ngầm định trong môi trường Node.js</h4>
<p>
    NPM giúp chúng ta quản lý và setup được các thư viện hỗ trợ của javascipt ( Mặc định khi setup Note JS, thì
    chương trình
    cũng ta tự động cài đặt NPM).
</p>
<p>
    Những câu lệnh thông dụng thường xuyên sử dụng, tham khảo tại ( https://docs.npmjs.com/cli/v6/commands )
</p>
<p>
    Câu lệnh cơ bản cũng rất quan trọng như "npm init" ( giúp ta setup tự động các môi trường thư viện trong
    project ).
</p>
<p>
    VD như: Nếu ta có 1 project và cần có nhiều người cùng phát triển trên project đó, làm sao ta có thể setup
    nhanh cácthư viện hỗ trợ 1 cách nhanh chóng dựa trên hệ điều hành mà ta chạy để chỉnh sửa Project đó.
</p>
<p>
    Câu lệnh "npm
    init" sẽ giúp ta bằng
    cách tạo ra 1 file là package.json, tại file này, chúng ta có thể cấu hình để cập nhật các thư viện của
    project đó cần.
    Khi 1 người khác edit project này trên 1 pc nơi khác, có thể cập nhật được những thư viện và môi trường
    giống
    nhau,
    để khi chỉnh sửa hoặc nâng cấp sẽ không gặp lỗi.
</p>
<h4>Package-lock.json</h4>
<p>
    File này sẽ ghi nhận chi tiết quá trình cài đặt các thư viện, khi setup càng nhiều thư viện, thì thông tin
    của file này
    sẽ dài ra thêm nhiều hơn, cũng như ghi nhận cài thêm các phụ thuộc của các thư việc cài đặt ghi nhận tại
    file package.json.
    file này chủ yếu cho máy đọc, ( không xóa )
</p>
<h4>Folder Node_modules</h4>
<p>
    Là nơi chứa các file của thư viện ( không được xóa), cũng không nên upload và share khi chúng ta share
    project với người khác.
    vì file này cấu hình dựa trên PC và hệ điều hành của người thực hiện project, nên khi chia sẽ file
    Node_modules,
    người thực hiện project này
    trên máy khác sẽ gặp lỗi, và dung lượng của file này cũng nặng.
</p>
<h4>Express JS</h4>
<p>
    Là 1 Framework web back end hỗ trợ cho Note JS, giúp ta tối ưu hóa code ngắn gọn hơn khi setup config, giúp
    thời gian phát triển ứng dụng nhanh, tối ưu hơn, và rất nhiều hỗ trợ khác,
    ( https://expressjs.com/en/starter/installing.html ) cũng như giúp lập trình bậc cao.
</p>
<h4>View Egines</h4>
<p>
    Là công cụ giúp chung ta viết code HTML một cách ngắn gọn hơn, hỗ trợ trong Data binding một cách hiệu quả,
    tối ưu hóa khi phát triển sản phẩm.
</p>
<h3 id="user-content-section22" dir="auto">2. Cơ Bản về Knockout.js</h3>
<p>
    Knockout(KO) là một thư viện của Javascript, nó giúp bạn tạo, hiển thị hay hiệu chỉnh User Interface(UI) với một
    data model được định nghĩa sẵn. Bất cứ khi nào bạn có phần thay đổi(thay đổi về action của user hay dữ liệu nội
    tại
    thay đổi) trong UI thì KO có thể giúp bạn thực hiện nó một cách đơn giản, và dễ kiểm soát. Hỗ trợ truy xuất
    database
    theo cách đơn giản, hữu dụng hơn. ( Data binding ).
</p>
<p>
    Mục đích chính cũng giúp chúng ta có để Loading dữ liệu theo thời gian thực trên Client.
</p>
<hr>
</hr>
<h3>Still Loading ...</h3>
