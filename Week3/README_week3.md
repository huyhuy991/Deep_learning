# Làm sạch và Biến đổi dữ liệu (Patient Heart Rate)

## Giới thiệu

Lab 3 tập trung vào kỹ năng tiền xử lý dữ liệu thực tế với bộ dữ liệu `patient_heart_rate.csv`. Nội dung chính bao gồm việc xử lý các lỗi dữ liệu phổ biến như thiếu tiêu đề, dữ liệu hỗn hợp, không thống nhất đơn vị, giá trị rỗng và trùng lặp.

---

## Công nghệ sử dụng

* **Ngôn ngữ**: Python
* **Thư viện chính**:
* `pandas`: Thao tác, biến đổi và làm sạch dữ liệu.
* `seaborn`: Hỗ trợ kiểm tra trực quan dữ liệu.


* **Môi trường**: Google Colab / Jupyter Notebook.

---

## Các vấn đề dữ liệu và Giải pháp xử lý

### Vấn đề 1: Thiếu tiêu đề (Missing Header)

* **Tình trạng**: File CSV không chứa dòng tiêu đề, dẫn đến việc dòng dữ liệu đầu tiên bị biến thành tiêu đề cột.
* **Giải pháp**: Định nghĩa danh sách `column_names` và tải lại dữ liệu với tham số `names` trong hàm `pd.read_csv`.

### Vấn đề 2: Dữ liệu hỗn hợp trong một cột (Multiple Variables in one column)

* **Tình trạng**: Cột `Name` chứa cả `Firstname` và `Lastname`.
* **Giải pháp**: Sử dụng hàm `.str.split()` để tách cột `Name` thành hai cột riêng biệt `Firstname` và `Lastname`, sau đó loại bỏ cột `Name` gốc.

### Vấn đề 3: Không thống nhất đơn vị đo lường (Inconsistent Unit)

* **Tình trạng**: Cột `Weight` chứa cả đơn vị `kgs` và `lbs`.
* **Giải pháp**: Duyệt qua các dòng, chuyển đổi các giá trị có đơn vị `lbs` sang `kgs` (chia cho 2.205) để đồng nhất dữ liệu.

### Vấn đề 4: Dòng dữ liệu rỗng (Null/NaN values)

* **Tình trạng**: Xuất hiện các dòng không có giá trị (NaN).
* **Giải pháp**: Sử dụng `dropna()` với tham số `how="all"` để xóa các dòng hoàn toàn trống.

### Vấn đề 5: Dữ liệu trùng lặp (Duplicate rows)

* **Tình trạng**: Có nhiều bản ghi giống hệt nhau cho cùng một bệnh nhân.
* **Giải pháp**: Sử dụng `drop_duplicates()` dựa trên các trường thông tin định danh để loại bỏ.

### Vấn đề 6: Ký tự lạ và lỗi font (Non-ASCII characters)

* **Tình trạng**: Cột tên chứa các ký tự có dấu hoặc ký tự đặc biệt do lỗi mã hóa.
* **Giải pháp**: Sử dụng biểu thức chính quy (regex) để loại bỏ các ký tự không thuộc bảng mã ASCII.

### Vấn đề 7: Xử lý giá trị thiếu (Missing values)

* **Tình trạng**: Nhiều cột `Age` và `Weight` bị thiếu giá trị.
* **Giải pháp**:
* Xóa các dòng thiếu cả `Age` và `Weight`.
* Thay thế các giá trị `Age` còn thiếu bằng giá trị trung bình (mean) của cột.



### Vấn đề 8: Biến đổi cấu trúc dữ liệu (Reshaping Data)

* **Tình trạng**: Cột `sex_and_time` chứa thông tin gộp giữa giới tính và khoảng thời gian đo nhịp tim.
* **Giải pháp**:
* Dùng `pd.melt()` để chuyển dữ liệu từ dạng bảng ngang (wide format) sang bảng dọc (long format).
* Sử dụng Regex để tách thông tin `Sex`, `hours_lower`, `hours_upper` từ cột hỗn hợp.



---

## Kết quả

* Sau quá trình xử lý, dữ liệu được chuẩn hóa và lưu vào file `patient_heart_rate_clean.csv`.
* Bộ dữ liệu sạch sẵn sàng cho các bước phân tích thống kê và trực quan hóa chuyên sâu.

---

## Cách chạy chương trình

1. Đảm bảo file `patient_heart_rate.csv` nằm trong cùng thư mục làm việc.
2. Thực thi tuần tự các cell trong file Notebook `2374802010190_TranMinhHuy_Lab3.ipynb`.

---

## Tác giả

* **Trần Minh Huy** - 2374802010190
