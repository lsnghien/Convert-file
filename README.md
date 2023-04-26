# Convert language to Vietnamese (https://github.com/vuvoth/Dapp-Learning/blob/51407f0542ab94bccb4e41b286ac778dcb1a489e/basic/01-web3js-deploy/README.md)
# Abtract
Thông qua những task cơ bản, bạn có thể tiếp thu những kiến thức liên quan đến trình biên dịch và quy trình triển khai một Smart Contract, cũng như làm thế nào để sử dụng các API cơ bản của `web3js`.
# Chuẩn bị
_ Tạo một dự án trên  [Infura](https://infura.io), và chọn `PROJECT ID`, sau đó thay đổi `ENDPOINTS` thành `Goerli`;

_ Tạo một account trên trình duyệt mở rộng `MetaMask`;
  1. Chọn `address` của ví và khóa riêng tư;
  2. Đến `Setting` - `advanced` và mở `Show test networks`;
     - Chọn `Goerli` và ghi nhận địa chỉ
  3. Nạp tiền vào tài khoản thông qua  [faucets](https://faucets.chain.link) hoặc các web dịch vụ khác;
  4. Sau vài phút có thể kiểm tra số dư trên `MetaMask`

_ Tạo một file `.env` và thêm các dòng sau:
  
    PRIVATE_KEY=YOUR_PRIVATE_KEY
    INFURA_ID=YOUR_PROJECT_ID
   
    
  | Ghi chú: Bạn có thể kiểm tra file `.env.example`
 
 _ Nếu bạn biết tiếng Trung bạn có thể kiểm tra các hoạt động này trên [BILIBILI](https://www.bilibili.com/video/BV1Y44y1r7E6/).
 
 # Bắt Đầu
 
 ## Hàm (functions) trong [Smart Contract](Incrementer.sol)
 - `Constructor`: Hàm khởi tạo (Constructor Function) được gọi khi smart contract được triển khai, đồng thời sẽ khởi tạo `số` (`number`) thành `số chuỗi đầu` (`_initialNumber`);
 
 - `increment`:   
