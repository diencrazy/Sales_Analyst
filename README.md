# 📊 Sales Analysis Dashboard (2016–2018)
Power BI Project • Retail Dataset • Data Analytics & BI

## ⭐ Giới thiệu
Dự án này phân tích dữ liệu bán hàng trong giai đoạn **2016–2018** với mục tiêu:
- Hiểu rõ hiệu suất kinh doanh theo thời gian
- Đánh giá đóng góp doanh thu theo sản phẩm, kênh bán hàng và khu vực
- Xác định cơ hội tối ưu chi phí và tăng trưởng
- Đưa ra insight và đề xuất chiến lược cho doanh nghiệp

Bộ dashboard được xây dựng bằng **Power BI**, với mục đích:
- Portfolio cá nhân
- Chuẩn bị phỏng vấn vị trí Data Analyst / BI Analyst
- Học thực hành Power BI từ A–Z

---

## 📁 Dataset
**Nguồn dữ liệu:** Provided by StartTrain (Entry Test)  
**Số bảng:** 4  
- **SalesManagement** (Fact): 72,743 records — chứa thông tin giao dịch
- **Region** (Dimension): 14 records — thông tin quốc gia và khu vực
- **SalesManagers** (Dimension): 14 records — Sales Manager theo quốc gia
- **Date** (Dimension): 1461 records – bảng ngày chuẩn hóa

---

## 🧱 Data Model (Star Schema)

```
          Region        SalesManagers
             \             /
              \           /
            SalesManagement  ---- Date
```

✔ Mô hình dạng **Star Schema**  
✔ Fact trung tâm + 3 Dimension  
✔ Quan hệ 1–n dựa trên Country và Date  

---

## 📊 Dashboard Overview

Dashboard gồm **7 trang**, bao gồm:

1️⃣ **Executive Summary**  
→ Tổng quan doanh thu, lợi nhuận, số đơn hàng, kênh bán hàng chủ lực

2️⃣ **Revenue Overview by Year/Month**  
→ Xu hướng doanh thu, mùa vụ, tăng trưởng YoY

3️⃣ **Product Performance**  
→ Doanh thu, số lượng bán, GPM theo từng dòng sản phẩm

4️⃣ **Product Type Deep Dive**  
→ Chi phí – giá bán – lợi nhuận từng product type

5️⃣ **Sales Channel Analysis**  
→ Web, Fax, Email, Local Store

6️⃣ **Region Analysis**  
→ Đánh giá doanh thu/GPM theo khu vực: Europe, Oceania, Latin America,…

7️⃣ **Manager / Country View**  
→ Hiệu suất theo Sales Manager

---

## 💡 Key Insights

### 🇪🇺 Europe – khu vực dẫn đầu doanh thu  
- Gần **$400M**, chiếm tỷ trọng lớn nhất  
- Tuy nhiên **GPM chưa tối ưu** → cơ hội cải thiện pricing/cost

### 🌏 Oceania & Latin America – thị trường tiềm năng  
- GPM cao nhất → khả năng thu hút lợi nhuận  
- Cần đầu tư marketing & mở rộng kênh phân phối

### 🛒 Web – kênh bán chủ lực  
- Chiếm **84% doanh thu**  
- Cần tối ưu chi phí vận hành và logistics

### 🎮 Video Games – sản phẩm bán chạy nhất  
- Hiệu suất cao, phù hợp mở rộng thêm SKU

---

## 🛠️ Kỹ thuật sử dụng

- Data Modeling (Star Schema)
- Power Query (Data Cleaning)
- DAX (Time Intelligence, Calculated Table/Column, KPI Metrics)
- Visualization & Data Storytelling
- Performance Optimization

### Một số DAX tiêu biểu

```DAX
Total Revenue = SUM(SalesManagement[Revenue])

Total Cost = SUM(SalesManagement[Unit Cost])

Gross Profit = [Total Revenue] - [Total Cost]

GPM % = DIVIDE([Gross Profit], [Total Revenue])

```

---

## 📌 Recommendations

1. **Tối ưu chi phí và logistics cho kênh Web**  
2. **Đầu tư marketing ở Oceania & Latin America**  
3. **Tối ưu chi phí sản phẩm (nhất là Mobile & Accessories)**  
4. **Tăng tồn kho trước mùa cao điểm quý 1 & 4**  

---

## 💻 File đính kèm
- `EntrytestDashboard.pbix` – File Power BI
- `Report.pdf` - File báo cáo phân tích dự án
- `README.md` – Mô tả dự án
- Tất cả file dữ liệu Excel: `*.xlsx`

---

## 👩‍💻 Author
**Đoàn Thị Kỳ Duyên**  
Liên hệ: doanthikyduyen2001@gmail.com  



