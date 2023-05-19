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
    * Switch Layer 2:
    Switch layer 2 về cơ bản là một cầu nối với nhiều port, mỗi port là một đoạn trong Ethernet LAN, biệt lập với các port còn lại. Việc truyền gói tin dựa hoàn toàn vào địa chỉ MAC hoặc địa chỉ IP chứa trong gói, nó sẽ không được truyền đi khi chưa biết được địa chỉ gốc.
    
       Việc truyền các gói tin trong Switch Layer 2 diễn ra như sau: gói tin được gửi từ một Host với một đích đến được đánh dấu bằng một địa chỉ MAC hoặc địa chỉ IP của máy đích. gói tin được gửi đến Switch Layer 2 và được lưu trong bộ nhớ tạm của Switch. Switch Layer 2 sẽ đọc thông tin đích đến là địa chỉ MAC hoặc địa chỉ IP của máy đích, sau đó nó sẽ lọc dữ liệu từ một bảng địa chỉ MAC và địa chỉ IP có sẵn để biết máy đích nằm ở cổng nào và sẽ chuyển tiếp gói tin này đến đúng cổng có địa chỉ MAC của máy đích.
    
       Việc thu thập và tạo bảng địa chỉ MAC và địa chỉ IP của Switch Layer 2 diễn ra như sau:
khi mạng được khởi chạy, Switch layer 2 sẽ bắn một gói tin Broadcast tới tất cả host trong mạng. các host này sẽ có quyền tiếp nhận hoặc không tiếp nhận gói tin Broadcast trên. nếu Host tiếp nhận, sau đó bắn trả lại một gói tin trả về cho Switch layer 2 thì Switch sẽ thu thập được các thông tin như địa chỉ IP, địa chỉ MAC của Host này và lưu trữ chúng lại trên một bảng với mục đích sử dụng để truy xuất dữ liệu về địa chỉ IP hoặc địa chỉ MAC cho các lần truyển tiếp gói tin trong mạng.

    * Switch layer 3
## Router
