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

<hr></hr>
<h3>I. Make first project with ASP .Net</h3>
<ol>
   <li><h4>Learn about file structure and test run
</li>
<div id="user-content-section1" dir="auto">

Chương trình sẽ bắt đầu chạy từ file Program.cs, tại file này chúng ta có thể

</div>

<p>

Tại thư mục đầu tiên là Connected Services sẽ làm việc khi chúng ta thêm 1 services bên ngoài vào ví dụ như: Cloud Storage with Azure Storage, …

Thư mục thứ 2 là: Dependencies

Thư mục thứ 3: Propeties, tại thư mục này chứa file launchSetting.json, file này sẽ chứa các profile để chúng ta thực thi ứng dụng ( Chúng ta có thể thấy tại nút play run chương trình màu xanh lá cây như IIS Express => khi kéo xuống chúng ta sẽ thấy Profile ISS Express + Tên Chính của Thư mục Profile chính )

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






