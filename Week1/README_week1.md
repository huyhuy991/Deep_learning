# Xét Tuyển Đại Học – Xử Lý Dữ Liệu

## Giới thiệu
Dự án này thực hiện xử lý dữ liệu xét tuyển đại học từ file CSV, bao gồm làm sạch dữ liệu, tính điểm xét tuyển theo từng khối thi và xuất kết quả ra file mới. Chương trình được viết và chạy trên Jupyter Notebook.

---

## Công nghệ sử dụng
- **Ngôn ngữ**: Python  
- **Thư viện**:
  - pandas
  - numpy
- **Môi trường**: Jupyter Notebook

---

## Cách hoạt động

### 1. Đọc dữ liệu
- Đọc dữ liệu từ file `dulieuxettuyendaihoc.csv`
- Sử dụng cột `STT` làm chỉ mục

### 2. Tiền xử lý dữ liệu
- Xử lý giá trị thiếu (`NaN`)
  - Cột `DT`: thay thế bằng `0`
  - Các cột điểm môn: thay thế bằng giá trị trung bình (Mean)

### 3. Xét tuyển
- Tính điểm xét tuyển dựa trên khối thi:
  - **Khối A, A1**  
    \[
    ((Môn 1 \times 2) + Môn 2 + Môn 3) / 4
    \]
  - **Khối B**  
    \[
    (Môn 1 + (Môn 2 \times 2) + Môn 3) / 4
    \]
  - **Khối khác**  
    \[
    (Môn 1 + Môn 2 + Môn 3) / 3
    \]

- Kết quả xét tuyển:
  - Điểm ≥ 5 → Đậu (`1`)
  - Điểm < 5 → Rớt (`0`)

- Kết quả được lưu trong cột `KQXT`

### 4. Xuất dữ liệu
- Lưu dữ liệu sau khi xử lý vào file:
  - `processed_dulieuxettuyendaihoc.csv`

---

## Kết quả
- Dữ liệu được làm sạch và chuẩn hóa
- Bổ sung cột `KQXT` thể hiện kết quả xét tuyển
- File đầu ra sẵn sàng cho việc thống kê hoặc phân tích tiếp theo

---

## Giao diện
- Không có giao diện web
- Chạy trực tiếp trên Jupyter Notebook
- Kết quả hiển thị trong notebook và file CSV đầu ra

---

## Cách chạy chương trình
1. Mở file notebook `2374802010190_TranMinhHuy.ipynb`
2. Đảm bảo file `dulieuxettuyendaihoc.csv` nằm cùng thư mục
3. Chạy lần lượt các cell trong notebook

---

## Tác giả
- Trần Minh Huy - 2374802010190
