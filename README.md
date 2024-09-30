* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f9f9f9;
}

.container {
    width: 1000px;
    margin: 20px auto;
    background-color: #fefefe;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    padding-bottom: 0px;
}

h2 {
    color: #0070c9;
    font-size: 20px;
    margin-bottom: 10px;
}

/* Bố cục hàng ngang cho ảnh chính */
.content-row {
    display: flex;
    justify-content: space-between;
}

.left-column {
    width: 65%;
}
.divider {
    height: 0.5px; /* Chiều cao của đường kẻ */
    background-color: #e0dddd; /* Màu xám nhẹ */
    width: 377px;
    position: relative; /* Đảm bảo vị trí tương đối */
    left: -39px; /* Dịch trái để căn chỉnh với ảnh main */
}
.main-image {
    position: relative;
    margin: 0; /* Đặt khoảng cách về 0 */
}

.main-image img {
    width: 100%; /* Đảm bảo chiều rộng đầy đủ */
    height: auto;
    display: block;
    margin: 0; /* Đặt khoảng cách về 0 */
    margin-left: -20px; 
}

.caption-box {
    background-color: #444; /* Màu xám đậm hơn */
    padding: 10px;
    text-align: left; /* Căn trái */
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%; /* Đặt chiều rộng bằng 100% của khung cha */
    box-sizing: border-box;
    margin-left: -20px; /* Xích khung xám qua trái một chút */
}

.caption {
    font-size: 16px;
    color: #fff;
    font-weight: bold;
}

.footer-text {
    font-size: 10px; /* Kích thước chữ nhỏ hơn */
    color: rgb(255, 255, 255); 
    position: absolute;
    bottom: 40px; /* Cách từ đáy ảnh để xích lên */
    right: 4px; /* Cách từ bên phải để di chuyển qua phải */
}

.right-column {
    width: 33%;
}

/* Bố cục cho các item bên phải */
.item.horizontal {
    display: flex;
    align-items: center; /* Căn chỉnh giữa */
    margin-bottom: 10px; /* Khoảng cách dưới mục này */
}

.item.horizontal img {
    width: 100px; /* Chiều rộng giảm */
    height: 60px; /* Chiều cao giảm */
    object-fit: cover; /* Đảm bảo hình ảnh không bị biến dạng */
    margin-right: 10px;
}

.item.horizontal p.title {
    font-size: 14px;
    color: #333;
    line-height: 1.5;
    margin-top: -35px;
}

/* Bố cục cho các item còn lại */
.right-column-items {
    display: flex;
    flex-direction: column; /* Sắp xếp dọc */
}

.right-column-items .item {
    display: flex;
    align-items: center;
    margin-bottom: 10px; /* Khoảng cách giữa các item */
}

.right-column-items .item img {
    width: 100px; /* Chiều rộng giảm */
    height: 60px; /* Chiều cao giảm */
    object-fit: cover; /* Đảm bảo hình ảnh không bị biến dạng */
    margin-right: 10px;
}

.right-column-items .item p {
    font-size: 14px;
    color: #333;
    line-height: 1.5;
    margin-top: 5px;
}
