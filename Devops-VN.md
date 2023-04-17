<h1>Learn about Load Balancer and Devops</h1>
<h2>About Load Balancer</h2>
<p>
    Load Balancer là cách phân phối lưu lượng hiệu quả trên nhiều máy chủ, Load Balancer
    giống như "cảnh sát giao thông" đứng trước máy chủ và định tuyến,
    có thể kiểm soát các yêu cầu của máy khách trên tất cả các máy chủ để có tốc
    độ và hiệu suất cao nhất và đảm bảo rằng không máy chủ làm việc quá sức..
</p>
<h2>About DevOps</h2>

<p>Devops là từ viết tắt của từ Developmet (Dev) => Người phát triển phần mềm + Operations (Ops) => Là Người Triển khai
    và
    cài đặt.
    Devops là kết nối giữa 2 công việc trên.</p>
<p>Người làm Devops không cần thiết phải làm việc viết phần mềm, nhưng ta phải biết được các khái niệm, luồng dữ liệu,
    và
    phải làm thế nào để phần mềm đó chạy được. VD như đội phát triễn sẽ đưa phần mềm và làm thế nào ta có thể setup cho
    phần
    mềm đó chạy như ở trên máy của đội phát triển chạy.</p>
<p>Và quan trọng người làm Devops phải biết được phần config ( Phần tùy biến như Databases, Web Services , Automation
    test,
    … ).</p>
<p>Giả sử như 1 ứng dụng đã viết xong, và đã test xong và cần được đẩy trên server nào đó để khách hàng sử dụng => Đây
    là
    trách nhiệm của Devops.</p>
<p>Người làm Depvops cũng phải biết các kiến thức về Networking, Security, DNS hoạt động như thế nào, những khái niệm
    liên
    quan
    tới virtualization…</p>


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
    <li>
        <h3><a href="#Section16">Application Load Balancer</a></h3>
    </li>
    <li>
        <h3><a href="#Section17">Software Load Balancers</a></h3>
    </li>
    <li>
        <h3><a href="#Section18">Hardware Load Balancers</a></h3>
    </li>
    <li>
        <h3><a href="#Section19">Virtual Load Balancers</a></h3>
    </li>
    <li>
        <h3><a href="#Section111">Public Load Balancers</a></h3>
    </li>
    <li>
        <h3><a href="#Section112">Private Load Balancers</a></h3>
    </li>
    <li>
        <h3><a href="#Section113">Azure Load Balancer</a></h3>
    </li>

</ol>
<h3><a href="#Section3">II. Website caching architecture</a></h3>
<h3><a href="#Section4">III. Monitoring & logging for services</a></h3>
<h3><a href="#Section2">IV. DevOps</a></h3>

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
    <p>
        Global Server Load Balancing (GSLB) là một công nghệ hướng lưu lượng truy cập mạng đến một nhóm trung tâm dữ
        liệu ở
        các vị trí địa lý khác nhau. Mỗi trung tâm dữ liệu cung cấp các dịch vụ ứng dụng tương tự và lưu lượng khách
        được
        hướng đến trang Web tối ưu với hiệu suất tốt nhất cho mỗi khách hàng. GSLB giám sát sức khỏe và sự đáp ứng của
        từng
        trang Web như Cân bằng tải máy chủ, hướng lưu lượng truy cập đến trang Web với thời gian phản hồi tốt nhất.
        GSLB cung cấp Cân bằng tải cho nhiều trang Web hoặc trung tâm dữ liệu bao gồm các dịch vụ sau:
    <p>
        – Khả năng khôi phục cao và khắc phục thảm họa và liên tục kinh doanh cho các môi trường có nhiều trang và trung
        tâm
        dữ liệu nằm ở các vị trí khác nhau. Nếu một trang Web không thành công, hệ thống GSLB phản hồi bằng cách chuyển
        hướng người dùng cuối và khách hàng đến các trang Web có sẵn thay thế.</p>
    <p>
        – Khả năng mở rộng được cung cấp, cho phép các tổ chức cung cấp dịch vụ từ nhiều trung tâm dữ liệu, được đặt ở
        các
        vị trí chiến lược ở bất kỳ đâu trên thế giới.</p>
    <p>– Hiệu suất đạt được bằng cách phân phối các yêu cầu tải công việc của khách hàng tới nhiều trang Web. Nhiệm vụ
        chính
        của Global Server Load Balancing là nhận biết vị trí địa lý và hướng các yêu cầu của khách hàng đến vị trí trung
        tâm
        dữ
        liệu gần nhất dựa trên địa lý hoặc hiệu suất mạng.</p>
    </p>
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
<h4>Pod là gì</h4>
<p>
    Pod là thành phần cơ bản nhất trong một hệ thống Kubernetes.
    Pod nằm trong các woker nodes là nơi chứa các container (một hay nhiều).
    Mỗi pod giống như một logic machine riêng biệt (có IP, hostname, tiếng trình riêng).
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
    www. Tên Miền .com sang một địa chỉ IP dạng số tương ứng với tên miền đó và ngược lại.
</p>
<h4>Container</h4>
<p>Container giống như 1 chuẩn mới, mà rất nhiều ứng dụng được đóng gói thành các container khác nhau, sau đó mới
    được
    Deploy lên server ( Sau đó ta có thể dùng các công nghệ để quản lý các Container này, tiêu biểu ví dụ như dùng
    Docker</p>

<h4 id="user-content-Section16" dir="auto">6. Application Load Balancer</h4>
<p>Application Load Balancer hỗ trợ quá trình cân
    bằng tải ứng dụng bằng cách sử dụng các giao thức HTTP và HTTPS (HTTP bảo mật).</p>

<h4 id="user-content-Section17" dir="auto">7. Software Load Balancers</h4>

<p>Software Load Balancer (SLB) là một giải pháp phần mềm cho phép phân phối tải các yêu cầu từ khách hàng đến các máy
    chủ phục vụ. Nó là một phần mềm được cài đặt trên một máy chủ ở giữa khách hàng và các máy chủ phục vụ
    và sử dụng các thuật toán phân phối tải để phân phối lưu lượng truy cập đến các máy chủ khác nhau.</p>

<p>Với SLB, một tập hợp các máy chủ phục vụ có thể được tổ chức thành một nhóm, gọi là pool. Các máy chủ trong pool có
    thể được cấu hình để chia sẻ tải lên nhau, điều này giúp giảm thiểu tình trạng quá tải trên một máy chủ và tăng khả
    năng khả năng chịu tải của hệ thống.</p>

<p>SLB là một giải pháp phần mềm linh hoạt hơn các giải pháp cứng (hardware) load balancer và có thể triển khai trên các
    máy chủ thông thường, giúp giảm thiểu chi phí đầu tư cho phần cứng.</p>

<h4 id="user-content-Section18" dir="auto">8. Hardware Load Balancers</h4>

<p>Hardware Load Balancer (HLB) là một thiết bị phần cứng được thiết kế để phân phối tải các yêu cầu từ khách hàng đến
    các máy chủ phục vụ. Nó là một thiết bị độc lập, được cài đặt ở giữa khách hàng và các máy chủ phục vụ và sử dụng
    các thuật toán phân phối tải để phân phối lưu lượng truy cập đến các máy chủ khác nhau.</p>
<p>Các HLB thường được cấu hình để tạo thành một nhóm máy chủ phục vụ có thể chia sẻ tải lên nhau, điều này giúp giảm
    thiểu tình trạng quá tải trên một máy chủ và tăng khả năng khả năng chịu tải của hệ thống. Các HLB cũng có thể được
    tích hợp với các tính năng bảo mật, như kiểm soát truy cập và mã hóa, để bảo vệ hệ thống khỏi các cuộc tấn công
    mạng.</p>
<p>Các HLB thường được sử dụng trong các môi trường doanh nghiệp lớn hoặc các ứng dụng web có lưu lượng truy cập cao. So
    với phần mềm Load Balancer, HLB có thể cung cấp khả năng xử lý lưu lượng truy cập lớn hơn và đáng tin cậy hơn vì nó
    được thiết kế để hoạt động trên phần cứng tốt hơn. Tuy nhiên, chi phí đầu tư và bảo trì cho HLB có thể cao hơn so
    với phần mềm Load Balancer.</p>

<h4 id="user-content-Section19" dir="auto">9. Virtual Load Balancers</h4>

<p>Virtual Load Balancer (VLB) là một giải pháp phần mềm để phân phối tải trên các ứng dụng và hệ thống mạng. Nó được
    triển khai dưới dạng ảo hóa trên một máy chủ vật lý hoặc trên một nền tảng điện toán đám mây. </p>
<p>VLB cung cấp khả năng phân phối tải đến các máy chủ ảo và vật lý, cũng như quản lý lưu lượng truy cập giữa các ứng
    dụng và dịch vụ khác nhau. Nó sử dụng các thuật toán phân phối tải để phân phối các yêu cầu đến các máy chủ phục vụ
    khác nhau và có thể cấu hình để cân bằng tải đối với các ứng dụng và dịch vụ khác nhau.</p>
<p>VLB cung cấp khả năng mở rộng linh hoạt và có thể được triển khai trong môi trường đám mây công cộng hoặc riêng tư.
    Nó có thể được cấu hình để hoạt động như một dịch vụ độc lập hoặc như một phần của một cụm hệ thống. VLB có thể là
    một giải pháp tốt cho các tổ chức muốn cân bằng tải và quản lý lưu lượng truy cập của họ trong môi trường ảo hóa và
    đám mây.</p>

<h4 id="user-content-Section111" dir="auto">10. Public Load Balancers</h4>

<p>Public Load Balancer (PLB) là một loại Load Balancer được triển khai trên một mạng công cộng như internet và được sử
    dụng để phân phối tải trên các ứng dụng hoặc dịch vụ trên các máy chủ được triển khai trên nhiều vùng địa lý khác
    nhau.</p>
<p>PLB có thể được sử dụng để phân phối tải cho các ứng dụng web, ứng dụng di động và các dịch vụ đám mây công cộng,
    chẳng hạn như Amazon Web Services, Microsoft Azure hay Google Cloud Platform. Nó sử dụng các thuật toán phân phối
    tải để phân phối các yêu cầu đến các máy chủ phục vụ khác nhau, giúp cân bằng tải và tăng khả năng khả năng chịu tải
    của hệ thống. </p>
<p>PLB có thể cung cấp các tính năng bảo mật, như kiểm soát truy cập và mã hóa, để bảo vệ hệ thống khỏi các cuộc tấn
    công mạng và cũng có thể hỗ trợ các tính năng như phân tích đăng nhập, giám sát và theo dõi hoạt động để giúp quản
    trị viên quản lý và giám sát hệ thống.</p>
<p>PLB là một giải pháp tốt cho các tổ chức muốn triển khai các ứng dụng hoặc dịch vụ của họ trên một mạng công cộng và
    muốn có khả năng mở rộng linh hoạt và cân bằng tải trên các máy chủ phục vụ được triển khai trên nhiều vùng địa lý
    khác nhau.</p>

<h4 id="user-content-Section112" dir="auto">11. Private Load Balancers</h4>

<p>Private Load Balancer (PrLB) là một giải pháp phân phối tải được triển khai trên một mạng riêng, chẳng hạn như một
    mạng doanh nghiệp, một mạng LAN (Local Area Network) hoặc một mạng VPN (Virtual Private Network).</p>
<p>PrLB được sử dụng để phân phối tải trên các ứng dụng và dịch vụ trên các máy chủ được triển khai trên một mạng riêng,
    giúp cân bằng tải và tăng khả năng chịu tải của hệ thống. Nó sử dụng các thuật toán phân phối tải để phân phối các
    yêu cầu đến các máy chủ phục vụ khác nhau, giúp tối ưu hóa hiệu suất của hệ thống.</p>
<p>PrLB cung cấp khả năng quản lý và giám sát lưu lượng truy cập giữa các ứng dụng và dịch vụ khác nhau, giúp quản trị
    viên quản lý và giám sát hệ thống. Nó cũng có thể được cấu hình để hoạt động như một dịch vụ độc lập hoặc như một
    phần của một cụm hệ thống. </p>
<p>PrLB là một giải pháp tốt cho các tổ chức muốn triển khai các ứng dụng hoặc dịch vụ của họ trên một mạng riêng và
    muốn có khả năng mở rộng linh hoạt và cân bằng tải trên các máy chủ phục vụ được triển khai trên một mạng riêng. Nó
    cũng cung cấp tính bảo mật cao hơn so với PLB vì nó được triển khai trên một mạng riêng được kiểm soát.</p>

<h4 id="user-content-Section113" dir="auto">12. Azure Load Balancer</h4>
<p>Azure Load Balancer là một dịch vụ phân phối tải được cung cấp bởi Microsoft Azure, giúp phân phối tải trên các ứng
    dụng và dịch vụ trên các máy chủ ảo trong một mạng ảo (Virtual Network) của Azure. Nó cung cấp khả năng cân bằng tải
    lưu lượng truy cập đến các máy chủ ảo (VMs) hoạt động trong mạng ảo và giúp tăng cường tính sẵn sàng và khả năng mở
    rộng của ứng dụng.</p>

<p>Azure Load Balancer có thể được cấu hình để hoạt động ở hai chế độ:</p>
<p>- Chế độ Basic: cung cấp tính năng phân phối tải cho các máy chủ ảo, với các thuật toán cân bằng tải Round Robin và
    Hash-based.</p>
<p>- Chế độ Standard: bên cạnh các tính năng của chế độ Basic, còn cung cấp các tính năng nâng cao hơn, bao gồm tính
    năng quản lý và giám sát lưu lượng truy cập, tính năng cân bằng tải dựa trên các thông tin TCP/UDP, tính năng cân
    bằng tải trên các dịch vụ hỗ trợ các giao thức không liên tục và khả năng kết nối phân tán trên các vùng địa lý khác
    nhau.</p>

<p>Azure Load Balancer là một trong những dịch vụ quan trọng của Microsoft Azure và được sử dụng rộng rãi để cân bằng
    tải trên các ứng dụng và dịch vụ hoạt động trên các máy chủ ảo trong mạng ảo của Azure.</p>

<h3 id="user-content-Section3" dir="auto">II. Website caching architecture</h3>
<P>
    Cache trên web là một ứng dụng công nghệ cho bộ nhớ tạm thời (caching) của các dữ liệu từ trang Web, ví dụ các trang
    HTML và các hình ảnh nhằm mục đích giảm lag khi server hoạt động. Một hệ thống bộ nhớ lưu trữ nhiều dữ liệu mà nó
    cho phép; các yêu cầu xuất hiện thêm như cần lưu trữ thêm sẽ được thực hiện nếu hệ thống này cho phép.


</P>
<p>
    Thay vì lúc nào bạn cũng phải bỏ thời gian tối ưu hóa máy tính thì việc sử dụng Web Cache giúp tăng được tốc độ load
    của server. Thử tưởng tượng đang có rất nhiều khách hàng, họ cùng có mối quan tâm đối với một trang Web. Ứng dụng sẽ
    hoạt động bằng cách lưu giữ các “bản sao” của các trang Web đó và sẽ đáp ứng các nhu cầu của người dùng bằng những
    “bản sao” giống hoàn toàn với bản chính mà không cần phải quay trở về Web nguồn. Việc quay trở về như thế sẽ làm
    server của Web hoạt động rất chậm, tình trạng “lag”, khiến cho khách hàng gần như mất thiện cảm với trang web của
    bạn.


</p>
<a href="https://longvan.net/web-cache-la-gi.html">Link tham khảo thêm</a>

<h3 id="user-content-Section4" dir="auto">III. Monitoring & logging for services</h3>
<p>
    Là hệ thống kiểm tra định kỹ, thường xuyên đo đạc các chỉ số của hệ thống, từ đó cung cấp cho chúng ta
    cái nhìn chính xác và tổng quan, tình trạng mà hệ thống đang hoạt động, giúp ta phát hiện các rủi ro gây hại cho
    hệ thống.
</p>

<h3 id="user-content-Section2" dir="auto">II. DevOps</h3>
<h4 id="user-content-Section21" dir="auto">1. Explain about container</h4>
<p>Container giống như 1 chuẩn mới, mà rất nhiều ứng dụng được đóng gói thành các container khác nhau, sau đó mới được
    Deploy lên server
    ( Sau đó ta có thể dùng các công nghệ để quản lý các Container này, tiêu biểu ví dụ như dùng Docker</p>
<p>VD như trong mỗi Pod sẽ quản lý được nhiều container, Kubernetes API sẽ không thể can thiệp vào container mà nó phải
    can thiệp vào container thông qua pod
</p>


<h4 id="user-content-Section22" dir="auto">2. Storage</h4>
<p>
<p>Storage còn gọi Bộ nhớ máy tính, thường được gọi là ổ nhớ (storage) hoặc bộ nhớ (memory), là một
    thiết bị công nghệ bao gồm các phần tử máy tính và lưu trữ dữ liệu, được dùng để duy trì dữ liệu số. Nó là một linh
    kiện cơ bản có chức năng cốt lõi của các máy tính.</p>

<p>Bộ nhớ máy tính bao gồm các bộ nhớ điện tĩnh (non-volatile memory) để lưu trữ được dữ liệu của máy tính một cách lâu
    dài (khi kết thúc một phiên làm việc của máy tính thì dữ liệu không bị mất đi), hoặc bộ nhớ điện động (volatile
    memory) để lưu dữ liệu tạm thời trong quá trình làm việc của máy tính (khi kết thúc một phiên làm việc của máy tính
    thì bộ nhớ này bị mất hết dữ liệu).</p>

<p>Các thiết bị lưu trữ dữ liệu cho bộ nhớ lâu dài bao gồm: Đĩa cứng, Đĩa mềm, Đĩa quang, Băng từ, ROM, các loại bút
    nhớ...</p>

<p>Các thiết bị lưu trữ dữ liệu tạm thời trong quá trình làm việc: RAM máy tính, Cache...</p>

<p>Hầu hết các bộ nhớ nêu trên thuộc loại bộ nhớ có thể truy cập dữ liệu ngẫu nhiên, riêng băng từ là loại bộ nhớ truy
    cập tuần tự.</p>

<p>Bộ nhớ máy tính có thể chia thành hai dạng: Bộ nhớ trong (main memory) và bộ nhớ ngoài (external storage).</p>
</p>

<h4 id="user-content-Section23" dir="auto">3. Network</h4>
<p>

<p>Network hay có thể hiểu là Mạng máy tính,là mạng viễn thông kỹ thuật số cho phép các nút mạng chia sẻ tài nguyên.
    Trong các mạng máy tính, các thiết bị máy tính trao đổi dữ liệu với nhau bằng các kết nối (liên kết dữ liệu) giữa
    các nút. Các liên kết dữ liệu này được thiết lập qua cáp mạng như dây hoặc cáp quang hoặc phương tiện không dây như
    Wi-Fi.</p>

<p>Các thiết bị máy tính mạng làm nhiệm vụ khởi động, định tuyến và chấm dứt dữ liệu được gọi là các nút mạng. Các
    nút thường được xác định bởi địa chỉ mạng và có thể bao gồm máy chủ mạng như máy tính cá nhân, điện thoại và máy
    chủ, cũng như phần cứng mạng như bộ định tuyến và chuyển mạch. Hai thiết bị như vậy có thể được cho là được kết nối
    với nhau khi một thiết bị có thể trao đổi thông tin với thiết bị kia, cho dù chúng có kết nối trực tiếp với nhau hay
    không. Trong hầu hết các trường hợp, các giao thức truyền thông dành riêng cho ứng dụng được xếp lớp (nghĩa là mang
    theo trọng tải) so với các giao thức truyền thông chung khác. Bộ sưu tập công nghệ thông tin ghê gớm này đòi hỏi
    phải có những người quản lý mạng lành nghề để giữ cho tất cả hệ thống mạng hoạt động tốt.</p>

<p>Mạng máy tính hỗ trợ một số lượng lớn các ứng dụng và dịch vụ như truy cập vào World Wide Web, video kỹ thuật số, âm
    thanh kỹ thuật số, sử dụng chung các máy chủ lưu trữ và ứng dụng, máy in và máy fax, và sử dụng email và ứng dụng
    nhắn tin tức thời cũng như nhiều ứng dụng khác. Mạng máy tính khác nhau về cách thức truyền tin được sử dụng để mang
    tín hiệu, giao thức truyền thông để tổ chức lưu lượng mạng, kích thước của mạng, cấu trúc liên kết, cơ chế điều
    khiển lưu lượng và ý định tổ chức mạng. Mạng máy tính nổi tiếng nhất là Internet.</p>
</p>

<h4 id="user-content-Section24" dir="auto">4. Policy</h4>
<p>
<p>Policy hay có thể hiểu là Network Policy
    Là công cụ chính để bảo mật kubernetes network. Nó cho phép ta dễ dàng giới hạn network traffic trong cluster để chỉ
    cho phép các traffic mong muốn đi qua.</p>

<p>Để hiểu tầm quan trọng của Network policies (chính sách mạng), hãy cùng tìm hiểu ngắn gọn về cách bảo mật mạng
    thường đạt được trước khi có network policy. Trước đây trong các mạng doanh nghiệp, bảo mật mạng được cung cấp bằng
    cách thiết kế cấu trúc liên kết vật lý của các thiết bị mạng (switch, router, firewall) và cấu hình liên quan của
    chúng. Cấu trúc liên kết vật lý xác định ranh giới bảo mật của mạng. Trong giai đoạn đầu tiên của ảo hóa, cùng một
    cấu trúc mạng và thiết bị mạng được ảo hóa trên đám mây và các kỹ thuật tương tự để tạo cấu trúc liên kết mạng cụ
    thể của các thiết bị mạng (ảo) đã được sử dụng để cung cấp bảo mật mạng. Việc thêm các ứng dụng hoặc dịch vụ mới
    thường yêu cầu thiết kế mạng bổ sung để cập nhật cấu hình mạng và cấu hình thiết bị mạng nhằm cung cấp bảo mật mong
    muốn.</p>

<p>Ngược lại, mô hình mạng Kubernetes xác định một mạng “flat” trong đó mỗi pod có thể giao tiếp với tất cả các pod
    khác trong cluster bằng địa chỉ IP của pod. Cách tiếp cận này đơn giản hóa hàng loạt thiết kế mạng và cho phép các
    workload mới được lập lịch động ở bất kỳ đâu trong cluster mà không phụ thuộc vào thiết kế mạng.</p>

<p>Trong mô hình này, thay vì bảo mật mạng được xác định bởi các ranh giới cấu trúc liên kết mạng, nó được xác định
    bằng cách sử dụng các chính sách mạng độc lập với cấu trúc liên kết mạng. Các chính sách mạng được đóng gói hơn nữa
    khỏi mạng bằng cách sử dụng label selector làm cơ chế chính của chúng để xác định workload nào có thể trao đổi với
    workload nào, thay vì địa chỉ IP hoặc dãy địa chỉ IP.</p>
</p>

<h4 id="user-content-Section25" dir="auto">5. Image Caching</h4>
<p>Ta có thể hiểu bằng cách tách 2 khái niệm này thành:</p>
<p>
    Image có thể hiểu là nơi hay môi trường cho ta lưu tất cả lại như source code, libs, file, tool, biến môi trường, hệ
    điều hành,...
    cũng là Base cấp thấp nhất, để cho các ứng dụng của mình có thể chạy lên nó. Ứng dụng cần những thứ gì thì Image sẽ
    gọp tất cả lại
</p>
<p>Caching là một kỹ thuật tăng độ truy xuất dữ liệu và giảm tải cho hệ thống. Cache là nơi lưu tập hợp các dữ liệu,
    thường có tính chất nhất thời, cho phép sử dụng lại dữ liệu đã lấy hoặc tính toán trước đó, nên sẽ giúp tăng tốc cho
    việc truy xuất dữ liệu ở những lần sau.</p>
<p>Từ đó ta có thể hiểu Image Caching là phương pháp có thể xử lý image 1 cách tối ưu hóa và nhanh nhất.</p>

<h4 id="user-content-Section26" dir="auto">6. Components of Kubernetes</h4>

<p>Giới thiều về Kubernetes: Đây là 1 cái tool open soure được phát triển bởi google, đóng vai trò đảm bảo các services,
    container hoạt
    động
    trơn tru theo
    hướng dẫn từ 1 file config có đuổi yaml, yml.</p>
<p>Kubernetes được xây dựng với 3 thành phần chính là Master, Node và các Addons</p>

<p>
<h4>- Đầu tiên là về thành phần Master</h4>

Thành phần này có thể xem là trái tim của Kubernetes, được xây dựng để quản lý tất cả các hoạt động, thao tác với
các containers trong cluster. Nó bao gồm API Server (kube-apiserver), etcd, Scheduler (kube-scheduler), Controller
Manager (kube-controller-manager) và Cloud Controller Manager (cloud-controller-manager).
</p>

<p>
<h4>- Thứ 2 là thành phần Node</h4>
Thành phần Node được xây dựng để chạy trên tất cả các node của Kubenetes cluster, chịu trách nhiệm quản lý và báo cáo
tình trạng của các Pods cho Kubernetes Master.
<p>Để làm được điều này, trong mỗi node, chúng ta sẽ có một agent tên là kubelet, chịu trách nhiệm quản lý và báo cáo
    các
    hoạt động của node về API Server của Kubernetes Master. kubelet sẽ chạy các container sử dụng container runtime như
    Docker. Nó sẽ không quản lý các container không được tạo bởi Kubernetes.</p>

</p>
<p>Một thành phần nữa trong Node đó là kube-proxy đảm nhiệm vai trò routing giữa service và các pods. Ở mỗi node,
    chúng ta cũng sẽ có các Container Runtime đảm nhận việc chạy các containers. Kubernetes hỗ trợ một vài container
    runtime như: Docker, rkt, …</p>
<p>
<h4>- Thành phần cuối cùng của Kubernetes là các Addons</h4>
<p>Thành phần này là các pods và service hiện thực các chức năng của một cluster như DNS Server, Web UI (Dashboard) hỗ
    trợ quản lý Kubernetes cluster bằng giao diện, Container Resource Monitoring (record các thông tin về hệ thống vào
    database và cho phép chúng ta phân tích các thông tin đó sử dụng UI) và Cluster-level Logging (lưu log của các
    container để chúng ta có thể xem thông tin log của chúng).</p>
</p>

<hr>
</hr>
<h3>Still Loading ...</h3>
