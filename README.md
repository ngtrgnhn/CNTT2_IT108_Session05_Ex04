### **Bảng so sánh Absolute Path và Relative Path**

| Tiêu chí | Absolute Path (Đường dẫn tuyệt đối)C:\\Users\\An-K26\\FarmProject\\data\\logs.csv | Relative Path (Đường dẫn tương đối)../data/logs.csv |
| :---- | :---- | :---- |
| Độ dài & Cấu trúc | Dài, cứng nhắc, phụ thuộc hoàn toàn vào cấu trúc cây thư mục gốc của ổ đĩa và tên tài khoản máy tính cụ thể. | Ngắn gọn, linh hoạt, tính từ vị trí thư mục hiện tại của file script đang chạy. |
| Tính di động (Portability) | Kém: Bị lỗi ngay lập tức khi chuyển project sang máy tính khác, đổi tên user (An-K26), hoặc đổi ổ đĩa (D: sang C:). | Cao: Dự án có thể dễ dàng sao chép sang máy tính khác, gửi cho đồng đội hoặc đưa lên Git mà không sợ bị gãy đường dẫn (miễn giữ nguyên cấu trúc nội bộ). |

### 

### **Lựa chọn tối ưu và ý nghĩa ký hiệu ..**

* Lựa chọn tối ưu: Sử dụng Relative Path (../data/logs.csv).  
* Giải thích ý nghĩa ký hiệu ..:  
  * Ký hiệu .. trong đường dẫn đại diện cho thư mục cha (parent directory) — tức là di chuyển lùi ra ngoài một cấp so với thư mục chứa file script hiện tại, sau đó truy cập vào thư mục data để đọc file logs.csv. Việc này giúp mã nguồn độc lập với môi trường hệ thống của từng cá nhân.

