# Tuần 6: Xây dựng mô hình phân loại hình ảnh FashionMNIST

## 📝 Giới thiệu
Nội dung tuần này tập trung vào việc làm quen với bài toán phân loại hình ảnh (Image Classification) bằng cách sử dụng bộ dữ liệu FashionMNIST. Dự án bao gồm các bước từ tiền xử lý dữ liệu đến xây dựng và huấn luyện mô hình mạng thần kinh cơ bản bằng PyTorch.

## 🚀 Nội dung thực hiện
- **Khởi tạo dữ liệu:** Tải bộ dữ liệu FashionMNIST trực tiếp từ `torchvision.datasets`.
- **Tiền xử lý:** - Xây dựng lớp `FMNISTDataset` tùy chỉnh.
    - Chia tỷ lệ dữ liệu (Normalization) bằng cách chia cho 255 để đưa giá trị pixel về đoạn [0, 1].
- **Xây dựng mô hình:** Thiết kế mạng Neural Network với các lớp `nn.Linear`, sử dụng hàm kích hoạt ReLU và kiến trúc đa tầng.
- **Huấn luyện:** - Sử dụng hàm tối ưu hóa SGD (Stochastic Gradient Descent).
    - Thiết lập DataLoader với `batch_size` phù hợp để tối ưu bộ nhớ.
- **Trực quan hóa:** Sử dụng `Matplotlib` để hiển thị các hình ảnh mẫu và kết quả dự đoán.

## 🛠 Công nghệ sử dụng
- **Ngôn ngữ:** Python
- **Framework:** PyTorch, Torchvision
- **Thư viện:** Numpy, Matplotlib

## 👤 Thông tin sinh viên
- **Họ tên:** Trần Minh Huy
- **MSSV:** 2374802010190
