<h1>Tìm Hiểu Về Công Nghệ Front End and Back End</h1>
<h2>Mục Lục</h2>
<h3><a href="#Section1">I. Tìm hiểu Về ASP.Net
    </a></h3>
<ol>
    <li>
        <h3><a href="#Section2">Tìm hiểu về cấu trúc dự liệu trong ASP.Net
            </a></h3>
    </li>
    <li>
        <h3><a href="#Section3">Tìm hiểu LinkQ
            </a></h3>
    </li>
</ol>
<h3><a href="#Section2">II. Tìm Hiểu Về Note.JS, Knockout.JS
    </a></h3>
<ol>
    <li>
        <h3><a href="#Section2">Cơ bản về Note JS</a></h3>
    </li>
    <li>
        <h3><a href="#Section3">Cơ bản về Knockout JS
            </a></h3>
    </li>
</ol>
<hr>
</hr>
<h3>I. Tìm hiểu Về ASP.Net</h3>
<ol>
    <li>
        <h4>Tìm hiểu về cấu trúc dự liệu trong ASP.Net</h4>
    </li>
    <div id="user-content-section1" dir="auto">
        Chương trình sẽ bắt đầu chạy từ file Program.cs, tại file này chúng ta có thể
    </div>
    <h4>Thư mục đầu tiên:</h4>
    <p> Connected Services sẽ làm việc khi chúng ta thêm 1 services bên ngoài vào ví dụ như: Cloud Storage with Azure
        Storage, …
    </p>
    <h4>Thư mục thứ 2:</h4>
    <p>
        Dependencies
    </p>
    <h4>Thư mục thứ 3:</h4>
    <p>
        Propeties, tại thư mục này chứa file launchSetting.json, file này sẽ chứa các profile để chúng ta thực thi ứng
        dụng ( Chúng ta có thể thấy tại nút play run chương trình màu xanh lá cây như IIS Express => khi kéo xuống chúng
        ta sẽ thấy Profile ISS Express + Tên Chính của Thư mục Profile chính ). Và cũng có thể setup đa mội trường tại
        đây. Và file này chỉ chạy trên Local, còn khi lên Server chủ yếu sẽ chạy vào các môi của appsetting.
    </p>
    <code>
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
</code>
    <h4>Thư mục thứ 4:</h4>
    <p>wwwroot là thư mục của ứng dụng, và tất cả như các file html, css, image, … đều đặt trong này.</p>

</ol>
<h2>II. Tìm Hiểu Về Note.JS, Knockout.JS</h2>
<ol>
    <h3>1. Cơ Bản về Note JS</h3>
    Note Js bản chất của nó là 1 cái vỏ bọc bên ngoài, nó giống 1 môi trường, nó không phải là 1 ngôn ngữ, không phải là
    Framework, là 1 môi trường giúp các bạn chạy được trên môi trường máy chủ bằng code javascript ( hỗ trợ từ C++ làm
    nền tảng kết nối với máy chủ )
    <h4>Kiến thức hỗ trợ để hiểu rõ hơn về Note JS</h4>
    <h4>Client - Server</h4>
    <p>
        - VD Client là gì, như các giao diện duyệt web như Chrome, Firefox, .., hay gọi là giao diện dành cho
        người dùng.
    </p>
    <p>
        - Server nơi sẽ phản hồi yêu cầu từ Client bằng Notejs ( dựa trên ngôn ngữ javascipt ), gửi về VD gói tin
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
</ol>
<h3>2. Cơ Bản về Knockout.js</h3>
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
