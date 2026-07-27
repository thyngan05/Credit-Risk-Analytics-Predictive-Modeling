# Credit-Risk-Analytics-Predictive-Modeling

## 🌟 Giới thiệu dự án (About Project)
Phân hệ đồ án ngành Công nghệ Thông tin, tập trung xây dựng hệ thống **Quản trị và Cảnh báo Sớm Rủi ro Tín dụng** cho ngân hàng. Dự án ứng dụng các kỹ thuật Khoa học Dữ liệu (Data Science) và Học máy (Machine Learning) nhằm tự động hóa quy trình thẩm định, dự báo nguy cơ vỡ nợ (nợ xấu) và hỗ trợ ban lãnh đạo ra quyết định kinh doanh chiến lược.

---

## 🛠️ Công nghệ sử dụng (Tech Stack)
* **Ngôn ngữ:** Python
* **Thư viện xử lý & Học máy:** Pandas, NumPy, Scikit-Learn, Imbalanced-Learn
* **Mô hình AI:** Logistic Regression, Random Forest Classifier
* **Trực quan hóa & Báo cáo:** Matplotlib, Seaborn, Microsoft Power BI
* **Môi trường phát triển:** Google Colab, VS Code

---

## 📂 Cấu trúc dự án (Project Structure)
```text
├── notebooks/                # Chứa source code Jupyter Notebook (.ipynb)
├── dashboards/               # Chứa file thiết kế báo cáo quản trị Power BI (.pbix)
└── screenshots/              # Hình ảnh minh họa giao diện Dashboard
```
🚀 Các bước thực hiện chính (Key Pipeline)
Tiền xử lý dữ liệu & Kiểm soát logic nghiệp vụ:

Xử lý dữ liệu khuyết bằng phương pháp Trung vị (Median) theo từng phân khúc Hạng tín dụng (Grade).

Lọc bỏ các bản ghi nhiễu vi phạm logic vòng đời tài chính (Tuổi, thâm niên, tỷ lệ vay vượt thu nhập).

Khám phá dữ liệu (EDA): Phân tích ma trận tương quan, trực quan hóa tác động của các biến định danh (Home, Intent, Grade) và phân phối mật độ tài sản.

Kỹ thuật đặc trưng (Feature Engineering): Rời rạc hóa dữ liệu phục vụ BI (Age_Group, Income_Group, Loan_Burden), mã hóa One-Hot/Ordinal và chuẩn hóa thang đo bằng Min-Max Scaling (chống rò rỉ dữ liệu).

Huấn luyện & So sánh mô hình: Xây dựng song song Logistic Regression và Random Forest (xử lý mất cân bằng nhãn với class_weight='balanced').

📊 Kết quả đạt được (Key Results)
Hiệu năng mô hình: Mô hình Random Forest đạt hiệu suất vượt trội với:

Accuracy (Độ chính xác chung): 92%

F1-Score (Nhóm nợ xấu): 0.79

AUC Score: 0.933 (Đạt độ tin cậy xuất sắc để tích hợp hệ thống tự động).

Phát hiện nghiệp vụ trọng tâm: Xác định chỉ số PercentIncome (Tỷ lệ gánh nặng trả nợ) là yếu tố quyết định số một chi phối nguy cơ vỡ nợ, vượt qua cả tổng thu nhập hay quy mô khoản vay.

📈 Giao diện Dashboard Power BI (Risk Command Center)
<img width="1998" height="1126" alt="image" src="https://github.com/user-attachments/assets/fd01f163-8d18-48c4-b189-f57f089375af" />
<img width="1996" height="1128" alt="image" src="https://github.com/user-attachments/assets/be7695f0-252a-4608-aa91-c3c876b1e702" />

