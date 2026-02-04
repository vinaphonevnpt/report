# 📊 Dashboard Phân Tích Doanh Thu Phát Triển Mới (PTM)  
### Trung tâm Khách hàng Doanh nghiệp 2 – Dịch vụ VTCNTT

---

## 🎯 Mục tiêu dự án

Xây dựng hệ thống Dashboard Power BI nhằm hỗ trợ Ban lãnh đạo:

- Theo dõi **doanh thu phát triển mới (PTM)** theo thời gian  
- So sánh giữa **doanh thu giao** và **doanh thu thực hiện**  
- Đánh giá hiệu quả theo **nhóm dịch vụ, LINE và AM**  
- Phát hiện kịp thời dịch vụ và khu vực cần cải thiện  

---

## 🧩 Phạm vi phân tích

Dashboard cho phép phân tích đa chiều theo:

- 📅 **Thời gian**: Tháng, Năm  
- 🧠 **Nhóm dịch vụ**  
- 🏢 **LINE kinh doanh**  
- 👤 **Nhân viên AM phụ trách**

---

## 🖥️ Cấu trúc Dashboard

### 1️⃣ KPI Tổng quan
Hiển thị nhanh các chỉ số quan trọng:

| KPI | Ý nghĩa |
|-----|--------|
| **Tổng doanh thu PTM** | Tổng doanh thu thực hiện PTM |
| **Tổng doanh thu giao** | Tổng giá trị giao chỉ tiêu |
| **Tỷ lệ PTM** | % thực hiện so với doanh thu giao |


---

### 2️⃣ Phân tích theo nhóm dịch vụ
Biểu đồ cột so sánh:

- 🔵 **Doanh thu PTM (thực hiện)**
- 🟦 **Doanh thu giao (kế hoạch)**

Giúp nhận diện:
- Dịch vụ vượt kế hoạch  
- Dịch vụ giao cao nhưng thực hiện thấp  

---

### 3️⃣ Phân tích cơ cấu & xu hướng

- 🥧 **Tỷ trọng thực hiện theo nhóm dịch vụ**
- 📈 **Xu hướng doanh thu PTM theo tháng**

---

## 🎛️ Bộ lọc phân tích

Dashboard hỗ trợ bộ lọc đồng bộ:

- LINE  
- Tên AM  
- Tháng  
- Năm  

Cho phép phân tích linh hoạt theo từng chiều kinh doanh.

---

## 🗂️ Kiến trúc dữ liệu

Hệ thống sử dụng mô hình **Star Schema** để tối ưu hiệu suất và độ chính xác:

### Fact Tables
- `khdn2_ptm` – Doanh thu thực hiện  
- `khdn2_khgiao` – Doanh thu giao  

### Dimension Tables
Bộ lọc thời gian hoạt động chính xác
- `dim_thoigian` – Thời gian (DateKey = YYYYMM)  
- `dim_nhomdichvu` – Nhóm dịch vụ chuẩn  
- `khdn2_dsam` – Thông tin AM & LINE  


---

## 📈 Giá trị mang lại

- Cung cấp bức tranh tổng thể về tình hình PTM  
- Hỗ trợ phát hiện điểm nghẽn kinh doanh  
- Đánh giá hiệu quả nhân sự AM  
- Theo dõi xu hướng doanh thu theo tháng  

---

## 🏢 Ứng dụng thực tế

Dashboard phục vụ:

- Họp giao ban kinh doanh định kỳ  
- Theo dõi hoàn thành chỉ tiêu  
- Phân bổ nguồn lực bán hàng  
- Đề xuất chiến dịch thúc đẩy dịch vụ trọng tâm  


---

## 📌 Ghi chú

Dự án được thiết kế để mở rộng trong tương lai, có thể bổ sung thêm:
- 
- Phân tích tình hình thanh toán của khách hàng đối với dự án đã nghiệm thu
- Phân tích tỷ lệ nộp hồ sơ gốc
- Dự báo doanh thu

---

**Tác giả:** Nhóm phân tích dữ liệu KHDN2  
**Công cụ sử dụng:** Power BI, SQL Server, Power Query, DAX
