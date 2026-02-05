# Lab 4: Làm sạch và Phân tích Dữ liệu Titanic (Titanic Disaster)

## Giới thiệu

Lab 4 tập trung vào các kỹ thuật tiền xử lý dữ liệu nâng cao và phân tích dữ liệu khám phá (EDA) trên bộ dữ liệu nổi tiếng về thảm họa tàu Titanic. Mục tiêu chính là xử lý các vấn đề về dữ liệu thiếu, định dạng lại dữ liệu và trích xuất các thông tin có ý nghĩa phục vụ cho việc phân tích.

---

## Công nghệ sử dụng

* **Ngôn ngữ**: Python.
* **Thư viện chính**:
* `pandas`: Thao tác, biến đổi và làm sạch dữ liệu.
* `seaborn` & `matplotlib`: Trực quan hóa dữ liệu để tìm ra các xu hướng.


* **Môi trường**: Google Colab / Jupyter Notebook.

---

## Nội dung thực hiện

### 1. Tải và Quan sát Dữ liệu

* Tải bộ dữ liệu `titanic_disaster.csv`.
* Sử dụng các hàm `head()`, `info()`, `describe()` để hiểu cấu trúc các biến: `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, và `Embarked`.

### 2. Xử lý Dữ liệu Thiếu (Missing Values)

* **Cột Age**: Thay thế các giá trị thiếu bằng giá trị trung bình (mean) của cột.
* **Cột Cabin**: Xử lý các giá trị thiếu.
* **Cột Embarked**: Điền các giá trị thiếu bằng phương pháp phù hợp.

### 3. Tiền xử lý và Chuẩn hóa Dữ liệu

* **Định dạng lại cột Name**: Trích xuất các danh xưng (Title) như Mr, Mrs, Miss... từ tên hành khách để phân tích sâu hơn.
* **Xử lý cột Sex**: Chuyển đổi dữ liệu dạng văn bản sang định dạng phù hợp cho phân tích.
* **Nhóm dữ liệu Age**: Chia hành khách thành các nhóm tuổi khác nhau (ví dụ: trẻ em, người lớn, người già).

### 4. Trực quan hóa và Phân tích Khám phá (EDA)

* Phân tích tỉ lệ sống sót dựa trên các yếu tố:
* **Giới tính (Sex)**: So sánh cơ hội sống sót giữa nam và nữ.
* **Hạng vé (Pclass)**: Xem xét tác động của hạng vé đến tỉ lệ sống sót.
* **Độ tuổi (Age)**: Phân tích sự phân bổ độ tuổi của những người sống sót và những người không may mắn.


* Sử dụng các loại biểu đồ: `countplot`, `histplot`, `boxplot` để thể hiện các mối liên hệ giữa các biến.

---

## Kết quả đạt được

* Hoàn thiện quy trình làm sạch dữ liệu cho một bộ dữ liệu thực tế phức tạp.
* Rút ra được các nhận định về các yếu tố ảnh hưởng lớn nhất đến khả năng sống sót trong thảm họa Titanic.
* Dữ liệu sau khi xử lý đã sẵn sàng cho các mô hình học máy (Machine Learning) ở các bước tiếp theo.

---

## Cách chạy chương trình

1. Đảm bảo file `titanic_disaster.csv` nằm trong cùng thư mục với notebook.
2. Cài đặt các thư viện cần thiết: `pip install pandas seaborn matplotlib`.
3. Thực thi tuần tự các cell trong file Notebook `2374802010190_TranMinhHuy_Lab4.ipynb`.

---

## Tác giả

* **Trần Minh Huy** - MSSV: 2374802010190.
