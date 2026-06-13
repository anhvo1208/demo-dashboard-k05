# **TechBank Vietnam \- HR Analytics Dashboard**

Đây là dự án **HR Analytics Dashboard** được xây dựng dành cho các chuyên gia Nhân sự (CHRO, HR Director, HR Team). Dashboard sử dụng kiến trúc hoàn toàn độc lập (serverless), chạy trực tiếp trên trình duyệt mà không cần cài đặt backend hoặc database phức tạp.

## **🌟 Tính năng nổi bật**

* **100% Serverless & Offline-first**: Upload file .xlsx và hệ thống tự động parse dữ liệu trực tiếp tại trình duyệt bằng thư viện SheetJS.  
* **Dynamic KPIs**: Tự động tính toán Tổng nhân sự (Active), Turnover Rate, Tỷ lệ tuyển dụng, Tỷ lệ giới tính và Điểm gắn kết theo thời gian thực.  
* **Modern UI/UX**: Giao diện chuẩn Enterprise với phong cách Glassmorphism (gương mờ), Dark theme tinh tế và Responsive cho mọi kích thước màn hình thiết bị.  
* **Advanced Charting**: Tích hợp Chart.js để hiển thị 05 biểu đồ phân tích đa chiều (Độ tuổi, Phòng ban, Lý do nghỉ việc...).  
* **Key Insights AI-like**: Tự động sinh ra các nhận xét quan trọng (Key Insights) từ dữ liệu sau khi người dùng lọc.

## **📂 Cấu trúc thư mục (Tối ưu cho GitHub Pages)**

Dự án được cố ý gộp chung HTML, CSS, và JS vào file index.html nhằm giúp người dùng có thể chạy trực tiếp bằng cách click đúp vào file mà không bị trình duyệt chặn bởi chính sách CORS (Cross-Origin Resource Sharing) khi truy xuất các module Javascript nội bộ.

/  
├── index.html        \# Main App (Giao diện \+ CSS Tailwind \+ JS Logic \+ ChartJS)  
├── README.md         \# Hướng dẫn chi tiết dự án  
└── LICENSE           \# Giấy phép MIT

## **🚀 Hướng dẫn cài đặt & Chạy cục bộ (Local)**

1. Tải toàn bộ source code về máy tính.  
2. Click đúp chuột vào file index.html để mở bằng trình duyệt (Khuyến nghị Google Chrome hoặc Edge).  
3. Tại màn hình Upload, chọn file dữ liệu mẫu Dataset.xlsx của bạn.  
4. Dashboard sẽ hiển thị ngay lập tức với các số liệu thực tế.

## **🌐 Hướng dẫn Deploy lên GitHub Pages (Miễn phí)**

Chỉ với 3 bước, bạn có thể public Dashboard này cho toàn công ty xem:

**Bước 1: Tạo Repository**

1. Đăng nhập vào [GitHub](https://github.com/).  
2. Nhấn nút **New Repository**. Đặt tên tùy ý (ví dụ: hr-analytics-dashboard).  
3. Đảm bảo để chế độ **Public**.  
4. Nhấn **Create repository**.

**Bước 2: Upload Files**

1. Tại màn hình repository vừa tạo, chọn **uploading an existing file**.  
2. Kéo thả 3 file index.html, README.md và LICENSE vào.  
3. (Tùy chọn) Kéo thả thêm file Dataset.xlsx nếu bạn muốn người khác có file mẫu để test thử.  
4. Bấm **Commit changes**.

**Bước 3: Kích hoạt GitHub Pages**

1. Trong repository của bạn, chuyển sang tab **Settings** (biểu tượng bánh răng).  
2. Ở menu bên trái, tìm và click vào mục **Pages**.  
3. Tại phần *Build and deployment*, mục *Source* giữ nguyên là **Deploy from a branch**.  
4. Tại mục *Branch*, chọn **main** (hoặc master), folder chọn **/(root)** và bấm **Save**.  
5. Đợi khoảng 1-2 phút, reload lại trang. Bạn sẽ thấy dòng chữ: *"Your site is live at https://\[username\].github.io/hr-analytics-dashboard/"*.  
6. Click vào link để trải nghiệm. Gửi link này cho sếp hoặc đồng nghiệp của bạn\!

## **🛠 Công nghệ sử dụng**

* **HTML5 & CSS3**  
* **Tailwind CSS** (via CDN)  
* **SheetJS** (xlsx.full.min.js) \- Đọc và xử lý file Excel phía Client.  
* **Chart.js** \- Vẽ biểu đồ tương tác.  
* **FontAwesome** \- Hệ thống Icon.

## **📝 Chú ý**

Toàn bộ dữ liệu Excel được upload **chỉ xử lý cục bộ trên RAM trình duyệt của bạn**. File của bạn không bị gửi đi hay lưu trữ trên bất kỳ server nào, đảm bảo an toàn bảo mật dữ liệu tuyệt đối (100% Data Privacy) cho doanh nghiệp.