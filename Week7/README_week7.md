# Tuần 7: Phân loại hình ảnh Chó và Mèo (Cats vs Dogs Classification)

## 📝 Giới thiệu
Dự án tuần này mở rộng bài toán phân loại hình ảnh sang bộ dữ liệu thực tế hơn là Cats vs Dogs. Mục tiêu chính là thực hiện các kỹ thuật xử lý ảnh phức tạp hơn và phân tích phân phối dữ liệu trước khi đưa vào huấn luyện.

## 🚀 Nội dung thực hiện
- **Kết nối dữ liệu:** Gắn thẻ (Mount) Google Drive để truy cập vào tập dữ liệu hình ảnh được lưu trữ.
- **Xử lý hình ảnh:** - Sử dụng thư viện `PIL` (Image) để mở và chuyển đổi định dạng ảnh.
    - Chuyển đổi ảnh sang dạng mảng Numpy và làm phẳng (flatten) dữ liệu.
- **Phân tích thống kê:**
    - Tính toán phân phối pixel của hình ảnh chó và mèo.
    - Vẽ biểu đồ **QQ-plot** (Quantile-Quantile plot) để kiểm tra xem dữ liệu hình ảnh có tuân theo phân phối chuẩn (Normal Distribution) hay không.
- **Kiến trúc mô hình:** Tiếp tục cải thiện mô hình CNN hoặc Deep Neural Network để thích ứng với kích thước hình ảnh biến động của tập dữ liệu thực tế.

## 🛠 Công nghệ sử dụng
- **Ngôn ngữ:** Python
- **Môi trường:** Google Colab
- **Framework:** PyTorch
- **Thư viện:** Pandas, Numpy, Scipy (stats), Matplotlib, PIL (Pillow), Glob.

## 👤 Thông tin sinh viên
- **Họ tên:** Trần Minh Huy
- **MSSV:** 2374802010190
