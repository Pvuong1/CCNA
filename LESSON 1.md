# Các thành phần cơ bản trong hệ thống mạng
* Các thành phần cơ bản trong hệ thống mạng bao gồm
## Máy tính
## Switch: 
* Switch là thiết bị chuyển mạch trong hệ thống mạng. Chúng được sử dụng để kết nối các đoạn mạng vào với nhau theo kiểu hình sao (Star). 
* Các loại switch
  * Phân loại theo tính năng:
    * Switch management: 
    Là dòng sản phẩm cho phép người dùng vào trong cấu hình. Mục đích của việc này là giúp thiết bị có thể hoạt động một cách linh hoạt hơn, tốt hơn và tính bảo mật cũng sẽ cao hơn.
    Việc quản lý Switch giúp người dùng tùy chỉnh thông số kỹ thuật sao cho phù hợp nhất với hệ thống mạng mà chúng ta đang sử dụng. Thông qua đó, chất lượng dịch vụ cũng sẽ được cải thiện một cách đáng kể.
    Switch quản lý chỉ sử dụng trong mạng có dây giúp kết nối cáp Ethernet thông qua một số thiết bị. Chúng cũng sẽ có công tắc điều chỉnh để thiết bị nói chuyện được với người khác.
    * Switch non-management:
    Sản phẩm này không cho phép người dùng điều chỉnh cấu hình. Chúng ta chỉ mua về và sử dụng theo như đúng cấu hình đã được cài đặt sẵn. Switch này phù hợp để sử dụng cho những kết nối đơn giản trong gia đình hoặc công ty, doanh nghiệp nhỏ.
  * Phân loại theo chức năng:
    * Workgroup Switch: 
    Là loại Switch được sử dụng để nối các máy tính lại với nhau từ đó tạo thành một mạng ngang hàng. Yêu cầu của Switch này không cần phải có tốc độ xử lý quá cao hay bộ nhớ quá lớn.
    * Segment Switch: 
    Được sử dụng để nối các Hub hoặc các Workgroup Switch với nhau. Điều này sẽ tạo nên liên kết ở tầng mạng thứ 2 của hệ thống. Yêu cầu của bộ Switch này đó là tốc độ xử lý phải cao.
    * Backbone Switch: 
    Được sử dụng để giúp kết nối các Segment Switch lại với nhau. Và yêu cầu là phải có bộ nhớ lớn cũng như tốc độ tải rất nhanh thì mới có thể chứa được tất cả các địa chỉ cho tất cả máy tính có trong hệ thống. Từ đó hoán chuyển dữ liệu một cách kịp thời giữa các mạng với nhau.
  * Phân loại theo lớp hoạt động:
    * Switch Layer 1:
    Là lớp cơ bản và là mô hình cổ nhất của switch. Ở thời kỳ sơ khai nó được gọi là Hub (bridge – bộ lặp). Một hub (một cổng vào, nhiều cổng ra), hoặc bộ lặp (một cổng vào, một cổng ra), là những thiết bị mạng đơn giản không quản lý bất kỳ lưu lượng truy cập nào đến qua nó. Bất kỳ gói tin nào được đưa vào Switch Layer 1 từ một cổng sẽ được “lặp lại” và được chuyển tới tất cả các thiết bị trong mạng qua các cổng khác ngoại trừ cổng nhập vào.
    * Switch Layer 2(Switch access):
    Switch layer 2 về cơ bản là một cầu nối với nhiều port, mỗi port là một đoạn trong Ethernet LAN, biệt lập với các port còn lại. Việc truyền gói tin dựa hoàn toàn vào địa chỉ MAC hoặc địa chỉ IP chứa trong gói, nó sẽ không được truyền đi khi chưa biết được địa chỉ gốc.
    
       Việc truyền các gói tin trong Switch Layer 2 diễn ra như sau: gói tin được gửi từ một Host với một đích đến được đánh dấu bằng một địa chỉ MAC hoặc địa chỉ IP của máy đích. gói tin được gửi đến Switch Layer 2 và được lưu trong bộ nhớ tạm của Switch. Switch Layer 2 sẽ đọc thông tin đích đến là địa chỉ MAC hoặc địa chỉ IP của máy đích, sau đó nó sẽ lọc dữ liệu từ một bảng địa chỉ MAC và địa chỉ IP có sẵn để biết máy đích nằm ở cổng nào và sẽ chuyển tiếp gói tin này đến đúng cổng có địa chỉ MAC của máy đích.
    
       Việc thu thập và tạo bảng địa chỉ MAC và địa chỉ IP của Switch Layer 2 diễn ra như sau:
khi mạng được khởi chạy, Switch layer 2 sẽ bắn một gói tin Broadcast tới tất cả host trong mạng. các host này sẽ có quyền tiếp nhận hoặc không tiếp nhận gói tin Broadcast trên. nếu Host tiếp nhận, sau đó bắn trả lại một gói tin trả về cho Switch layer 2 thì Switch sẽ thu thập được các thông tin như địa chỉ IP, địa chỉ MAC của Host này và lưu trữ chúng lại trên một bảng với mục đích sử dụng để truy xuất dữ liệu về địa chỉ IP hoặc địa chỉ MAC cho các lần truyển tiếp gói tin trong mạng.

    * Switch layer 3 (Switch core):
    Switch layer 3 về cơ bản, là sự kết hợp khả năng định tuyến của Router và thêm vào Switch layer 2 tiêu chuẩn. Sự khác biệt chính giữa hoạt động chuyển tiếp gói tin của một bộ định tuyến và sự ch Router (bộ định tuyến) là thiết bị mạng có chức năng chuyển tiếp gói dữ liệu giữa các mạng máy tính. Có thể hiểu, router thực hiện "chỉ đạo giao thông" trên Internet. Dữ liệu được gửi đi trên Internet dưới dạng gói, ví dụ như trang web hay email. Gói dữ liệu sẽ được chuyển tiếp từ router này đến router khác thông qua các mạng nhỏ, được kết nối với nhau để tạo thành mạng liên kết, cho đến khi gói dữ liệu đến được điểm đích.  uyển đổi lớp 3 là thực thi thực tế. Trong các router có mục đích chung, việc chuyển tiếp thường được thực hiện trong phần mềm chạy trên bộ vi xử lý hoặc bộ xử lý mạng , trong khi đó công tắc lớp 3 thực hiện cùng một hoạt động bằng phần cứng mạch tích hợp dành riêng cho ứng dụng chuyên dụng (ASIC).
    
      Switch layer 3 về cơ bản, là sự kết hợp khả năng định tuyến của Router và thêm vào Switch layer 2 tiêu chuẩn. Sự khác biệt chính giữa hoạt động chuyển tiếp gói tin của một bộ định tuyến và sự chuyển đổi lớp 3 là thực thi thực tế. Trong các router có mục đích chung, việc chuyển tiếp thường được thực hiện trong phần mềm chạy trên bộ vi xử lý hoặc bộ xử lý mạng , trong khi đó công tắc lớp 3 thực hiện cùng một hoạt động bằng phần cứng mạch tích hợp dành riêng cho ứng dụng chuyên dụng (ASIC).
## Router
* Router (bộ định tuyến) là thiết bị mạng có chức năng chuyển tiếp gói dữ liệu giữa các mạng máy tính. Có thể hiểu, router thực hiện "chỉ đạo giao thông" trên Internet. Dữ liệu được gửi đi trên Internet dưới dạng gói, ví dụ như trang web hay email. Gói dữ liệu sẽ được chuyển tiếp từ router này đến router khác thông qua các mạng nhỏ, được kết nối với nhau để tạo thành mạng liên kết, cho đến khi gói dữ liệu đến được điểm đích. 
* Các giao thức định tuyến của router
  * Open Shortest Path First (OSPF) - được sử dụng để tìm đường dẫn tốt nhất cho các gói, khi chúng đi qua một tập hợp các mạng được kết nối. OSPF được chỉ định bởi Internet Engineering Task Force (IETF) - một trong số các Interior Gateway Protocol (IGP).
  * Border Gateway Protocol (BGP) - quản lý cách các gói được định tuyến trên Internet thông qua việc trao đổi thông tin giữa các edge router. BGP cung cấp sự ổn định mạng, đảm bảo router có thể nhanh chóng thích ứng để gửi các gói thông qua một kết nối lại khác, nếu một đường dẫn Internet gặp sự cố.
  * Interior Gateway Routing Protocol (IGRP) - xác định cách thông tin định tuyến giữa các cổng sẽ được trao đổi trong một mạng tự trị. Thông tin định tuyến sau đó có thể được sử dụng bởi các giao thức mạng khác để chỉ định cách thức truyền tải nên được định tuyến. 
  * Enhanced Interior Gateway Routing Protocol (EIGRP) - phát triển từ IGRP. Nếu một router không thể tìm thấy đường đến đích ở một trong các bảng này, nó sẽ truy vấn lần lượt các bảng neighbor cho đến khi tìm thấy một tuyến đường mới. Khi một mục trong bảng định tuyến thay đổi ở một trong các router, nó sẽ thông báo về sự thay đổi cho các neighbor thay vì gửi toàn bộ bảng.
  * Exterior Gateway Protocol (EGP) - xác định cách thông tin định tuyến giữa hai neighbor gateway host (mỗi host có router riêng) được trao đổi. EGP thường được sử dụng giữa các máy chủ trên Internet để trao đổi thông tin bảng định tuyến.
  * Routing Information Protocol (RIP) - giao thức ban đầu để xác định cách router nên chia sẻ thông tin khi di chuyển lưu lượng giữa một nhóm mạng cục bộ được kết nối với nhau. Số hop lớn nhất được phép cho RIP là 15, giới hạn kích thước của mạng mà RIP có thể hỗ trợ.
