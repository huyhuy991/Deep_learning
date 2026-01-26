# Xét Tuyển Đại Học – Thống Kê và Trực Quan Hóa Dữ Liệu (Tuần 2)

## Giới thiệu

Tiếp nối quá trình làm sạch dữ liệu ở tuần 1, dự án tuần 2 tập trung vào việc sử dụng các kỹ thuật thống kê mô tả, bảng xoay dữ liệu (Pivot Table) và các công cụ trực quan hóa để phân tích sâu hơn về kết quả học tập và các yếu tố ảnh hưởng đến điểm thi của thí sinh.

---

## Công nghệ sử dụng

* **Ngôn ngữ**: Python
* **Thư viện**:
* `pandas`, `numpy`: Thao tác và biến đổi dữ liệu.
* `matplotlib`, `seaborn`: Trực quan hóa dữ liệu (biểu đồ đường, cột, tròn, hộp...).
* `scipy`, `statsmodels`: Hỗ trợ phân tích thống kê và kiểm tra phân phối.


* **Môi trường**: Jupyter Notebook / Google Colab.

---

## Cách hoạt động

### 1. Thống kê mô tả và Sắp xếp

* Đọc dữ liệu đã qua tiền xử lý từ file `processed_dulieuxettuyendaihoc.csv`.
* Thực hiện sắp xếp thí sinh theo điểm thi (`DH1`, `DH2`) và giới tính để quan sát thứ hạng.
* Sử dụng **Pivot Table** để tính toán các chỉ số: `count`, `sum`, `mean`, `median`, `min`, `max`, `std` và các tứ phân vị (`Q1`, `Q2`, `Q3`) dựa trên Khối thi (`KT`) và Khu vực (`KV`).

### 2. Phân tích nhóm dữ liệu

* Phân tích cơ cấu giới tính (`GT`) và dân tộc của thí sinh.
* Chuyển đổi điểm trung bình môn từ thang điểm 10 (Việt Nam) sang thang điểm 4 (Mỹ) bằng phương pháp chuẩn hóa.
* Phân lớp dữ liệu môn Toán (`T1`) thành các mức: Kém, Trung bình, Khá, Giỏi.

### 3. Trực quan hóa dữ liệu

* **Biểu đồ cột (Bar) & Tròn (Pie)**: Trình bày tỉ lệ giới tính và phân lớp học lực.
* **Biểu đồ Đường (Line)**: Khảo sát sự biến thiên của điểm số.
* **Biểu đồ Hộp (Boxplot)**: Xác định giá trị ngoại lai (outliers) và khoảng biến thiên điểm số theo từng nhóm khu vực.
* **Biểu đồ Histogram & Q-Q Plot**: Kiểm tra phân phối của dữ liệu có tuân theo phân phối chuẩn hay không.

### 4. Phân tích tương quan

* Sử dụng biểu đồ phân tán (**Scatter Plot**) và **FacetGrid** để tìm mối liên hệ giữa điểm thi đại học và điểm học tập lớp 12 theo từng khu vực.

---

## Kết quả

* Hiểu rõ cấu trúc phân bố điểm thi của thí sinh.
* Xác định được mối liên hệ giữa khu vực, giới tính và kết quả thi đại học thông qua hình ảnh trực quan.
* File đầu ra sẵn sàng cho các mô hình dự báo học tập nâng cao.

---

## Giao diện

* Không có giao diện web.
* Kết quả đồ họa hiển thị trực tiếp trong notebook (Inline plots) và các báo cáo thống kê dạng bảng.

---

## Cách chạy chương trình

1. Mở file notebook `2374802010190_TranMinhHuy_week2.ipynb`.
2. Đảm bảo file dữ liệu `processed_dulieuxettuyendaihoc.csv` (kết quả của tuần 1) nằm cùng thư mục.
3. Cài đặt các thư viện cần thiết: `pip install pandas matplotlib seaborn scipy statsmodels`.
4. Chạy lần lượt các cell để quan sát biểu đồ và bảng thống kê.

---

## Tác giả

* Trần Minh Huy - MSSV: 2374802010190
