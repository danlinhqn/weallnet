<h1>Learn about Load Balancer</h1>
<p>
    Mô tả: Load Balancer là cách phân phối lưu lượng hiệu quả trên nhiều máy chủ, Load Balancer
    giống như "cảnh sát giao thông" đứng trước máy chủ và định tuyến,
    có thể kiểm soát các yêu cầu của máy khách trên tất cả các máy chủ để có tốc
    độ và hiệu suất cao nhất và đảm bảo rằng không máy chủ làm việc quá sức..
</p>

<h2>Mục Lục</h2>
<h3><a href="#Section1">I. Có bao nhiêu loại LoadBalancer</a></h3>
<ol>
    <li>
        <h3><a href="#Section11">Global server load balancing</a></h3>
    </li>
    <li>
        <h3><a href="#Section12">Server Load Balancing</a></h3>
    </li>
    <li>
        <h3><a href="#Section13">Network Load Balancing</a></h3>
    </li>
    <li>
        <h3><a href="#Section14">Container Load Balancing</a></h3>
    </li>
    <li>
        <h3><a href="#Section15">Cloud Load Balancing</a></h3>
    </li>
</ol>
<h3><a href="#Section2">II. DevOps</a></h3>

<ol>
    <li>
        <h3><a href="#Section21">Explain about container</a></h3>
    </li>
    <li>
        <h3><a href="#Section22">Storage</a></h3>
    </li>
    <li>
        <h3><a href="#Section23">Network</a></h3>
    </li>
    <li>
        <h3><a href="#Section24">Policy</a></h3>
    </li>
    <li>
        <h3><a href="#Section25">Image Caching</a></h3>
    </li>
    <li>
        <h3><a href="#Section26">Components of Kubernetes</a></h3>
    </li>
</ol>

<hr>
</hr>

<h3 id="user-content-Section11" dir="auto">I. Có bao nhiêu loại LoadBalancer</h3>

<h4 id="user-content-section1" dir="auto">1. Global server load balancing</h4>
<div>
    Global server load balancing (cân bằng tải máy chủ toàn cầu – GSLB) có thể mở rộng khả năng của một trong hai
    loại trên nhiều trung tâm dữ liệu để có thể phân phối lưu lượng lớn một cách hiệu quả.
</div>

<h4 id="user-content-Section12" dir="auto">2. Server Load Balancing</h4>
<div>
    Global server load balancing (cân bằng tải máy chủ toàn cầu – GSLB) có thể mở rộng khả năng của một trong hai
    loại trên nhiều trung tâm dữ liệu để có thể phân phối lưu lượng lớn một cách hiệu quả.
</div>

<h4 id="user-content-Section13" dir="auto">3. Network Load Balancing</h4>
<div>
    Sẽ phân chia các lượng truy cập giữa các ip, switch, router
    Dùng ở tầng 4 ( Transpost ), nâng cao tính ổn định, Điều đó có nghĩa là chúng có thể đưa ra các quyết định định
    tuyến dựa trên các cổng TCP hoặc UDP mà các gói sử dụng cùng với địa chỉ IP nguồn và đích của chúng.
</div>

<h4 id="user-content-Section14" dir="auto">4. Container Load Balancing</h4>
<div>
    Container Load Balancing cung cấp các phiên bản ảo hóa, riêng biệt.
    Phổ biến nhất hiện nay là hệ thống Kubernetes orchestration,
    hệ thống này có thể phân chia load giữa các container pods với nhau để giúp nâng cao tính sẵn sàng.
</div>

<h4 id="user-content-Section15" dir="auto">5. Cloud Load Balancing</h4>
<div>
    Trong hạ tầng cloud, sẽ có nhiều sự lựa chọn cho việc cân bằng tải của mình, cũng có bao gồm cả: Server Load
    Balancing, Network Load Balancing
</div>

<h4>Thông tin tìm hiểu thêm để hiểu rõ về LoadBalancer</h4>
<h4>- Cổng TCP</h4>
<p>TCP (Transmission Control Protocol) là một giao thức mạng dùng trong truyền dữ liệu qua một mạng khác, được
    nhận xét là khá quan trọng. Một giao thức trong phạm vi mạng bao gồm những quy tắc và thứ tự quản lý quá
    trình truyền dữ liệu sao cho người dùng trên toàn cầu dù ở đâu, trên nền tảng gì, phần mềm nào đều được phép
    thao tác theo cùng một phương thức tương tự nhau thì được gọi là TCP.
    ( Truyển tin có kiểm tra -> Tốc độ thấp )
    ( Tin cậy hơn )</p>

<h4>- Cổng UDP</h4>
<p>
    UDP (User Datagram Protocol) được định nghĩa là giao thức dữ liệu người dùng, đây là giao thức giao tiếp
    thay thế cho giao thức mạng truyền dữ liệu TCP (Transmission Control Protocol), UDP được áp dụng vào việc
    tùy chỉnh, cài đặt những kết nối có độ trễ thấp và không chịu lỗi giữa các ứng dụng ở môi trường internet.
    ( Truyền tin không kiểm tra -> Tốc độ cao )
</p>

<h4>- Mô hình OSI</h4>
<p>
    Mô hình kết nối các hệ thống mở OSI là mô hình căn bản về các tiến trình truyền thông, thiết lập các tiêu chuẩn
    kiến
    trúc mạng ở mức Quốc tế, là cơ sở chung để các hệ thống khác nhau có thể liên kết và truyền thông được với nhau.
    Mô
    hình OSI tổ chức các giao thức truyền thông thành 7 tầng, mỗi một tầng giải quyết một phần hẹp của tiến trình
    truyền
    thông, chia tiến trình truyền thông thành nhiều tầng và trong mỗi tầng có thể có nhiều giao thức khác nhau thực
    hiện
    các nhu cầu truyền thông cụ thể.
</p>
<div>
    <table border="3">
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
                    <p style="text-align:justify">Chuyển đổi cú pháp dữ liệu để đáp ứng yêu cầu truyền thông của các
                        ứng
                        dụng</p>
                </td>
                <td>
                    <p style="text-align:justify">Giao thứcBiến đổi mã</p>
                </td>
            </tr>
            <tr>
                <td>
                    <p style="text-align:justify"><strong>5 - Session</strong></p>
                </td>
                <td>
                    <p style="text-align:justify">Quản lý các cuộc liên lạc giữa các thực thể bằng cách thiết lập,
                        duy
                        trì,
                        đồng bộ hóa và hủy bỏ các phiên truyền thông giữa các ứng dụng</p>
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
                    <p style="text-align:justify">Vận chuyển thông tin giữa các máy chủ (End to End). Kiểm soát lỗi
                        và
                        luồng
                        dữ liệu</p>
                </td>
                <td>
                    <p style="text-align:justify">Giao thức Giao vận</p>
                </td>
            </tr>
            <tr>
                <td>
                    <p style="text-align:justify"><strong>3 – Network</strong></p>
                </td>
                <td>
                    <p style="text-align:justify">Thực hiện chọn đường và đảm bảo trao đổi thông tin trong liên mạng
                        với
                        công nghệ chuyển mạch thích hợp.</p>
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
                    <p style="text-align:justify">Tạo/gỡ bỏ khung thông tin (Frames), kiểm soát luồng và kiểm soát
                        lỗi.
                    </p>
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
                    <p style="text-align:justify">Đảm bảo các yêu cầu truyền/nhận các chuỗi bit qua các phương tiện
                        vật
                        lý.
                    </p>
                </td>
                <td>
                    <p style="text-align:justify">Giao diện DTE - DCE</p>
                </td>
            </tr>
        </tbody>
    </table>
</div>
<h4>Congestion Control</h4>
<h4>Pods là gì</h4>
<p>
    Pods là thành phần cơ bản nhất trong một hệ thống Kubernetes.
    Pods nằm trong các woker nodes là nơi chứa các container (một hay nhiều).
    Mỗi pods giống như một logic machine riêng biệt (có IP, hostname, tiếng trình riêng).
</p>
<h4>Giao thức truyền tải file đơn giản (TFTP)</h4>
<p>
    TFTP là viết tắt của Trivial File Transfer Protocol, là 1 giao thức truyền file đơn giản, cho phép client có thể
    upload hoặc download các tệp tin từ trên các remote host như switch, router, server... TFTP được thiết kế nhỏ và
    dễ
    thực hiện, và do đó nó thiếu hầu hết các tính năng nâng cao của các giao thức truyền tệp. TFTP chỉ đọc và ghi
    tệp từ
    các máy chủ từ xa. Nó không thể liệt kê, xóa, hoặc đổi tên các tập tin hoặc thư mục và cũng không có xác thực
    giữa
    client và server.
</p>
<p>
    Do không được bảo mật trong quá trình truyền tệp nên TFTP thường được ứng dụng trong mạng cục bộ (LAN) để
    backup,
    import config IOS trên các thiết bị switch router firewall, hoặc cài đặt license cho các thiết bị này.
</p>
<p>
    TFTP sử dụng giao thức UDP làm giao thức truyền tải của nó và sử dụng port 69 làm port mặc định. Các tệp tin sẽ
    được
    chia nhỏ thành các Block có chiều dài cố định 512 byte và được truyền lần lượt. Cả 2 thiết bị đều có thể coi là
    1
    TFTP server hay TFTP Client (gọi chung là Remote Host).
</p>
<h4>Giao thức truyền tin thời gian thực (RTSP)</h4>
<p>
    RTSP là một giao thức điều khiển truyền thông mạng ở tầng ứng dụng.
    Nó giao tiếp với máy chủ đa phương tiện để thiết lập phiên
    và gửi các lệnh như “Tạm dừng” và “Phát” thay vì truyền dữ liệu dưới dạng luồng thực tế.
    Theo truyền thống, hầu hết các máy chủ RTSP cũng
    sử dụng RTP (Real Time Transfer Protocol) và RTCP (RTP Control Protocol)
    để phân phối các luồng dữ liệu đa phương tiện của chúng.
</p>
<p>Với quá nhiều lợi ích, RTSP được sử dụng cho nhiều mục đích khác nhau như thuyết trình trực tiếp,
    các trang web camera IP, học trực tuyến và nghe FM qua Internet.
    Sau đó, nó tiếp tục được đưa vào các nền tảng đa phương tiện hàng đầu như YouTube và Spotify,
    các ứng dụng truyền thông như Skype và trình phát đa phương tiện VLC.</p>
<h4>Hệ thống phân giải tên miền (DNS)</h4>
<p>
    DNS là viết tắt của cụm từ Domain Name System, mang ý nghĩa đầy đủ là hệ thống phân giải tên miền. DNS được phát
    minh vào năm 1984 cho Internet, chỉ một hệ thống cho phép thiết lập tương ứng giữa địa chỉ IP và tên miền.
</p>
<p>
    DNS là viết tắt của cụm từ Domain Name System, mang ý nghĩa đầy đủ là hệ thống phân giải tên miền. Hiểu một cách
    ngắn gọn nhất, DNS cơ bản là một hệ thống chuyển đổi các tên miền website mà chúng ta đang sử dụng, ở dạng
    www.tenmien.com sang một địa chỉ IP dạng số tương ứng với tên miền đó và ngược lại.
</p>
<h4>Container</h4>
<p>Container giống như 1 chuẩn mới, mà rất nhiều ứng dụng được đóng gói thành các container khác nhau, sau đó mới
    được
    Deploy lên server ( Sau đó ta có thể dùng các công nghệ để quản lý các Container này, tiêu biểu ví dụ như dùng
    Docker</p>

<div id="DevOps">
    <h3 id="user-content-Section21" dir="auto">II. DevOps</h3>
    <h4 id="user-content-Section22" dir="auto">1. Global server load balancing</h4>
    <p>
        Là hệ thống giống như kiểm tra định kỹ, thường xuyên đo đạc các chỉ số của hệ thống, từ đó cung cấp cho chúng ta
        cái nhìn chính xác tình
        trạng mà hệ thống đang hoạt động, giúp ta phát hiện các rủi ro gây hại cho hệ thống
    </p>
    <h4 id="user-content-Section23" dir="auto">2. Storage</h4>
    <h4 id="user-content-Section24" dir="auto">3. Network</h4>
    <h4 id="user-content-Section25" dir="auto">4. Policy</h4>
    <h4 id="user-content-Section26" dir="auto">5. Image Caching</h4>
    <h4 id="user-content-Section26" dir="auto">6. Components of Kubernetes</h4>
</div>

<hr>
</hr>
<h3>Still Loading ...</h3>
