Xét Tuyển Đại Học – Thống Kê và Trực Quan Hóa Dữ Liệu (Tuần 2)
Giới thiệu
Tiếp nối quá trình làm sạch dữ liệu ở tuần 1, dự án tuần này tập trung vào việc sử dụng các kỹ thuật thống kê mô tả, bảng xoay dữ liệu (Pivot Table) và các công cụ trực quan hóa (Matplotlib, Seaborn) để phân tích sâu hơn về kết quả học tập và xét tuyển của các thí sinh.

Công nghệ sử dụng
Ngôn ngữ: Python

Thư viện chính:

pandas: Thao tác và biến đổi dữ liệu.

numpy: Xử lý toán học và tính toán phân vị.

matplotlib & seaborn: Trực quan hóa dữ liệu (biểu đồ đường, cột, tròn, hộp...).

scipy & statsmodels: Hỗ trợ phân phối thống kê và biểu đồ Q-Q plot.

Môi trường: Jupyter Notebook / Google Colab.

Nội dung thực hiện
1. Thống kê mô tả và Sắp xếp dữ liệu
Đọc dữ liệu đã xử lý từ file processed_dulieuxettuyendaihoc.csv.

Sắp xếp thứ tự thí sinh dựa trên điểm thi đại học (DH1, DH2) theo các tiêu chí tăng dần và theo nhóm giới tính.

Sử dụng Pivot Table để tổng hợp các giá trị: count, sum, mean, median, min, max, std và các tứ phân vị (Q1, Q2, Q3) của điểm thi theo Khối thi (KT) và Khu vực (KV).

2. Phân tích theo nhóm dữ liệu
Thống kê số lượng thí sinh theo giới tính (GT).

Phân tích dữ liệu điểm trung bình hệ Mỹ (US_TBM) qua các năm.

Trích xuất dữ liệu riêng biệt cho nhóm thí sinh nam, dân tộc Kinh và có điểm thi đạt ngưỡng yêu cầu.

3. Trực quan hóa dữ liệu
Biểu đồ Bar & Pie: Thể hiện tỉ lệ giới tính thí sinh.

Biểu đồ Unstacked: So sánh xếp loại học lực (XL1, XL2, XL3) của học sinh nữ qua 3 năm.

Biểu đồ Đường (Line chart): Khảo sát sự biến thiên của điểm môn Toán (T1).

Biểu đồ Hộp (Box plot): Xác định giá trị ngoại lai và khoảng phân bố điểm số.

Biểu đồ Histogram: Xem tần suất xuất hiện của các khoảng điểm.

Q-Q Plot: Kiểm tra xem phân phối điểm số có tiệm cận phân phối chuẩn hay không.

4. Phân lớp dữ liệu
Tạo biến mới phanlopt1 để phân loại điểm môn Toán (T1) thành các mức: Kém, Trung bình, Khá, Giỏi.

Trực quan hóa mối tương quan giữa điểm thi đại học và điểm trung bình lớp 12 theo từng Khu vực bằng FacetGrid.

Kết quả đạt được
Hiểu rõ cấu trúc phân bố điểm thi của thí sinh qua các biểu đồ thống kê.

Xác định được mối liên hệ giữa khu vực, giới tính và kết quả thi đại học.

Báo cáo chi tiết các chỉ số thống kê quan trọng phục vụ cho việc dự báo kết quả tuyển sinh.

Cách chạy chương trình
Đảm bảo đã có file dữ liệu processed_dulieuxettuyendaihoc.csv trong cùng thư mục.

Cài đặt các thư viện cần thiết: pip install pandas numpy matplotlib seaborn scipy statsmodels.

Mở file 2374802010190_TranMinhHuy_week2.ipynb và thực thi các cell nội dung.

Tác giả
Trần Minh Huy - MSSV: 2374802010190
