<h1>Learn about Load Balancer</h1>
<p>
Description: Load Balancer is the way for efficient distribution of traffic on multiple servers, a Load Balancer as like "traffic cop" stay front of server and routing, can control requests of client on all server for the most speed and performance and ensure that no server is overworked.
</p>
 
<h3>How many types of LoadBalancer are there ?</h3>


<ol>
   
   <li><a href="#Section1">Global server load balancing</a></li>
   <li><a href="#Section2">Server Load Balancing</a></li>
   <li><a href="#Section3">Network Load Balancing</a></li>
   <li><a href="#Section4">Network Load Balancing</a></li>
   <li><a href="#Section5">Cloud Load Balancing</a></li>
</ol>


<h3>Purpose of using each type of LoadBalancer</h3>




<ol>
   
   <li><h4>Global server load balancing</li>
<div id="user-content-section1" dir="auto">

Global server load balancing (cân bằng tải máy chủ toàn cầu – GSLB) có thể mở rộng khả năng của một trong hai loại trên nhiều trung tâm dữ liệu để có thể phân phối lưu lượng lớn một cách hiệu quả.

</div>


<li><h4>Server Load Balancing</h4></li>
<div id="user-content-section2" dir="auto">

Global server load balancing (cân bằng tải máy chủ toàn cầu – GSLB) có thể mở rộng khả năng của một trong hai loại trên nhiều trung tâm dữ liệu để có thể phân phối lưu lượng lớn một cách hiệu quả.

</div>


<li><h4>Network Load Balancing</h4></li>
<div id="user-content-section3" dir="auto">

Sẽ phân chia các lượng truy cập giữa các ip, switch, router
Dùng ở tầng 4 (  Transpost ), nâng cao tính ổn định, Điều đó có nghĩa là chúng có thể đưa ra các quyết định định tuyến dựa trên các cổng TCP hoặc UDP mà các gói sử dụng cùng với địa chỉ IP nguồn và đích của chúng.

</div>
<li><h4>Container Load Balancing</h4></li>
<div id="user-content-section4" dir="auto">

Container Load Balancing cung cấp các phiên bản ảo hóa, riêng biệt. 
Phổ biến nhất hiện nay là hệ thống Kubernetes orchestration, 
hệ thống này có thể phân chia load giữa các container pods với nhau để giúp nâng cao tính sẵn sàng.

</div>
<li><h4>Cloud Load Balancing</h4></li>
<div id="user-content-section5" dir="auto">

Trong hạ tầng cloud, sẽ có nhiều sự lựa chọn cho việc cân bằng tải của mình, cũng có bao gồm cả: Server Load Balancing, Network Load Balancing

</div>

</ol>


<h3>Information learn more</h3>


<ol>




<li><h4>Cổng TCP</h4>
<p>TCP (Transmission Control Protocol) là một giao thức mạng dùng trong truyền dữ liệu qua một mạng khác, được nhận xét là khá quan trọng. Một giao thức trong phạm vi mạng bao gồm những quy tắc và thứ tự quản lý quá trình truyền dữ liệu sao cho người dùng trên toàn cầu dù ở đâu, trên nền tảng gì, phần mềm nào đều được phép thao tác theo cùng một phương thức tương tự nhau thì được gọi là TCP.
 ( Truyển tin có kiểm tra -> Tốc độ thấp )
( Tin cậy hơn )</p>
</li>


<li><h4>Cổng UDP</h4>
<p>
UDP (User Datagram Protocol) được định nghĩa là giao thức dữ liệu người dùng, đây là giao thức giao tiếp thay thế cho giao thức mạng truyền dữ liệu TCP (Transmission Control Protocol), UDP được áp dụng vào việc tùy chỉnh, cài đặt những kết nối có độ trễ thấp và không chịu lỗi giữa các ứng dụng ở môi trường internet.
 ( Truyền tin không kiểm tra -> Tốc độ cao )
</p>
</li>


<li><h4>Mô hình OSI</h4>


<p>
<tbody>
		<tr>
			<td>
			<p style="text-align:justify"><strong>Tầng</strong></p>
			</td>
			<td>
			<p style="text-align:justify"><strong>Chức năng chủ yếu</strong></p>
			</td>
			<td>
			<p style="text-align:justify"><strong>Giao thức</strong></p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>7 – Application</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Giao tiếp người và môi trường mạng</p>
			</td>
			<td>
			<p style="text-align:justify">Ứng dụng</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>6 – Presentation</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Chuyển đổi cú pháp dữ liệu để đáp ứng yêu cầu truyền thông của các ứng dụng</p>
			</td>
			<td>
			<p style="text-align:justify">Giao thức</p>


			<p style="text-align:justify">Biến đổi mã</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>5 - Session</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Quản lý các cuộc liên lạc giữa các thực thể bằng cách thiết lập, duy trì, đồng bộ hóa và hủy bỏ các phiên truyền thông giữa các ứng dụng</p>
			</td>
			<td>
			<p style="text-align:justify">Giao thức phiên</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>4 – Transpost</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Vận chuyển thông tin giữa các máy chủ (End to End). Kiểm soát lỗi và luồng dữ liệu</p>
			</td>
			<td>
			<p style="text-align:justify">Giao thức</p>


			<p style="text-align:justify">Giao vận</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>3 – Network</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Thực hiện chọn đường và đảm bảo trao đổi thông tin trong liên mạng với công nghệ chuyển mạch thích hợp.</p>
			</td>
			<td>
			<p style="text-align:justify">Giao thức mạng</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>2 – Data Link</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Tạo/gỡ bỏ khung thông tin (Frames), kiểm soát luồng và kiểm soát lỗi.</p>
			</td>
			<td>
			<p style="text-align:justify">Thủ tục kiểm soát</p>
			</td>
		</tr>
		<tr>
			<td>
			<p style="text-align:justify"><strong>1 - Physical</strong></p>
			</td>
			<td>
			<p style="text-align:justify">Đảm bảo các yêu cầu truyền/nhận các chuỗi bit qua các phương tiện vật lý.</p>
			</td>
			<td>
			<p style="text-align:justify">Giao diện DTE - DCE</p>
			</td>
		</tr>
	</tbody>


</p>
</li>


<li><h4>HTTP, HTTPS, SSL ( TLS ) -> Chứng chỉ bảo mật</h4></li>


<li><h4>Kiến ​​trúc Client-server</h4></li>


<li><h4>Congestion Control </h4></li>


<li><h4>Pods là gì</h4>
<p>
Pods là thành phần cơ bản nhất trong một hệ thống Kubernetes. 
Pods nằm trong các woker nodes là nơi chứa các container (một hay nhiều). 
Mỗi pods giống như một logic machine riêng biệt (có IP, hostname, tiếng trình riêng).




</p>
</li>


<li><h4>Giao thức truyền tải file đơn giản (TFTP)</h4></li>


<li><h4>Giao thức truyền tin thời gian thực (RTSP)</h4></li>


<li><h4>Giao thức liên mạng đơn giản (SNP)</h4></li>


<li><h4>Hệ thống phân giải tên miền (DNS)</h4></li>




</ol>



<hr></hr>
<h3>Still Loading ...</h3>








