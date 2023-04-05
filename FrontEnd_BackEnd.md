<h1>Learn about Front End and Back End</h1>
<h2>Outline</h2>

 <h3><a href="#Section1">I. Make first project with ASP .Net
</a></h3>


<ol>
   <li><h3><a href="#Section2">Learn about file structure and test run
</a></h3></li>
   <li><h3><a href="#Section3">Learn about LinkQ
</a></h3></li>
</ol>


 <h3><a href="#Section2">II. Tìm Hiểu Về Note.JS, Knockout.JS
</a></h3>


<ol>
   <li><h3><a href="#Section2">Cơ bản về Note JS</a></h3></li>
   <li><h3><a href="#Section3">Cơ bản về Knockout JS
</a></h3></li>
</ol>

<hr></hr>
<h3>I. Make first project with ASP .Net</h3>
<ol>
   <li><h4>Learn about file structure and test run
</li>
<div id="user-content-section1" dir="auto">


Chương trình sẽ bắt đầu chạy từ file Program.cs, tại file này chúng ta có thể

</div>

<p>



<h4>Thư mục đầu tiên:</h4>
<p> Connected Services sẽ làm việc khi chúng ta thêm 1 services bên ngoài vào ví dụ như: Cloud Storage with Azure Storage, …
</p>

<h4>Thư mục thứ 2:</h4>
<p>
Dependencies
</p>
<h4>Thư mục thứ 3:</h4>
<p>
Propeties, tại thư mục này chứa file launchSetting.json, file này sẽ chứa các profile để chúng ta thực thi ứng dụng ( Chúng ta có thể thấy tại nút play run chương trình màu xanh lá cây như IIS Express => khi kéo xuống chúng ta sẽ thấy Profile ISS Express + Tên Chính của Thư mục Profile chính ). Và cũng có thể setup đa mội trường tại đây. Và file này chỉ chạy trên Local, còn khi lên Server chủ yếu sẽ chạy vào các môi của appsetting.
</p>

<pre >
<h3>
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
</h3>
</pre>

<h4>Thư mục thứ 4:</h4>
<p>
wwwroot là thư mục của ứng dụng, và tất cả như các file html, css, image, … đều đặt trong này.
1</p>

<h2>II. Tìm Hiểu Về Note.JS, Knockout.JS</h2>

<h3>1. Cơ Bản về Note JS</h3>

Note Js bản chất của nó là 1 cái vỏ bọc bên ngoài, nó giống 1 môi trường, nó không phải là 1 ngôn ngữ, không phải là Framework, là 1 môi trường giúp các bạn chạy được trên môi trường máy chủ = code javascript ( hỗ trợ từ C++ )

<h3>Kiến thức hỗ trợ để hiểu rõ hơn về Note JS</h3>

<ol>
   <li><h4>Client - Server</h4></li>
	<p>
VD client là gì, như là các giao diện duyệt web như Chorme, Firefox, .., giao diện dành cho người dùng.

Server nơi sẽ respont yêu cầu từ client của ta sẽ viết = Notejs ( ngôn ngữ javascipt ), gửi về vd như ( html,csss, javascript, … )
	</p>
   <li><h4>NPM - chương trình quản lý thư viện ngầm định trong môi trường Node.js</h4></li>
</ol>

Client - Server




npm: trang cung cap’ nguon tai lieu ho tro javascript, npm giup quan ly va setup duoc cac thu vien voi javascript 9 ( Mac dinh khi setup notejs auto da~ cai` dat luon npm ) -> Nhung cau lenh thuong xuyen dung tham khao tai day ( https://docs.npmjs.com/cli/v6/commands )

Cau lenh co ban de setup thu vien nhu: npm init ( giup setup cac thu vien moi truong project ), VD nhu: nhieu cung` code 1 project, lam` sao de? co’ 1 moi truong` giong nhau de? cung` nhau edit, thi npm giup’ ta dieu do = cach tao ra 1 file package.json ( su dung = cau lenh tren CMD or Terminal is : npm init )

Package-lock.json ( File nay ghi nhan chi tiet lai qua trinh cai` dat cac thu vien, khi setup cac nhieu thu vien vao` thi file nay` se~ cang dai`, cung~ ghi nhan cai` dat them cac phu. thuoc. cua cac thu vien cai` dat ghi nhan tai. file package.json,  cai’ nay chu? yeu ghi cho may doc, khong xoa ) 

Node_modules: la noi chua cac file cua thu vien ( Khong dc xoa ‘ ) ( Cung~ khong nen share thu muc nay` neu’ nhieu` nguoi` cung` lam viec. tren 1 project ) ( co’ the? dung cau lenh npm install de? setup thu vien sau khi co’ source code, cac coder shard voi nhau tren 1 project ) ( file nay` phu thuoc vao he dieu hanh nguoi` share code + dung luong cao, rat de gay ra error cho nguoi` nhan source code )

=> cung~ la co che khi cung` nhau share source code voi nhau

Express ( Main thing ) ( la` 1 Framework web back end for notejs, giup viet code ngan gon hon khi setup config, giup thoi gian phat trien ung toi uu hon va` rat nhieu ho tro khac, phat trien ung dung nhanh hon ) ( https://expressjs.com/en/starter/installing.html ) giup coder lap trinh bac cao )

View Egines:  giup’ coder co’ the viet html + code cho vong` lap, code nguon` tren file html also hay if else, …

// —----------------->

Tìm hiểu về knockout.js

Mô Tả:

Knockout(KO) là một thư viện của Javascript, nó giúp bạn tạo, hiển thị hay hiệu chỉnh User Interface(UI) với một data model được định nghĩa sẵn. Bất cứ khi nào bạn có phần thay đổi(thay đổi về action của user hay dữ liệu nội tại thay đổi) trong UI thì KO có thể giúp bạn thực hiện nó một cách đơn giản, và dễ kiểm soát. Hỗ trợ truy xuất database theo cách đơn giản, hữu dụng hơn. ( Data binding )

<hr></hr>


<h3>Still Loading ...</h3>
