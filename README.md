# -n-KHDL-nh-m-5
## Cấu trúc thư mục 
```text
Credit-Card-Fraud-Detection/
│
├── dataset/                         # Quản lý dữ liệu
│   ├── raw/                         # Dữ liệu gốc tải từ Kaggle
│   │   └── creditcard.csv
│   └── processed/                   # Dữ liệu sau khi xử lý
│
├── notebooks/                       # Phân tích và thử nghiệm ML
│   ├── 01_Data_Collection.ipynb     # Thu thập và đọc dữ liệu
│   ├── 02_EDA.ipynb                 # Khám phá và trực quan hóa dữ liệu
│   ├── 03_Data_Preprocessing.ipynb  # Tiền xử lý dữ liệu
│   ├── 04_Imbalance_Handling.ipynb  # Xử lý mất cân bằng dữ liệu
│   ├── 05_Model_Training.ipynb      # Huấn luyện các mô hình
│   ├── 06_Model_Optimization.ipynb  # Tối ưu mô hình
│   └── 07_Model_Evaluation.ipynb    # Đánh giá và so sánh mô hình
│
├── src/                             # Source code Machine Learning
│   ├── __init__.py                  # Khởi tạo Python package
│   ├── preprocessing.py             # Xử lý và chuẩn hóa dữ liệu
│   ├── sampling.py                  # SMOTE, ADASYN, Undersampling...
│   ├── models.py                    # Xây dựng các mô hình ML
│   └── evaluation.py                # Các hàm đánh giá mô hình
│
├── models/                          # Lưu mô hình đã huấn luyện
│   ├── best_model.pkl               # Mô hình dự đoán tốt nhất
│   ├── scaler.pkl                   # Bộ chuẩn hóa dữ liệu
│   └── model_metadata.json          # Thông tin mô hình
│
├── frontend/                        # Giao diện người dùng (Streamlit)
│   ├── app.py                       # File chạy giao diện chính
│   │
│   ├── pages/                       # Các trang giao diện
│   │   ├── 1_Dashboard.py           # Trang tổng quan hệ thống
│   │   ├── 2_Fraud_Detection.py     # Trang phát hiện gian lận
│   │   └── 3_Model_Evaluation.py    # Trang đánh giá mô hình
│   │
│   ├── components/                  # Thành phần giao diện dùng chung
│   │   ├── sidebar.py               # Thanh điều hướng
│   │   ├── charts.py                # Các biểu đồ
│   │   └── metrics.py               # Hiển thị các chỉ số
│   │
│   ├── assets/                      # Tài nguyên giao diện
│   │   ├── css/
│   │   │   └── style.css            # Tùy chỉnh giao diện
│   │   └── images/                  # Logo, icon, hình ảnh
│   │
│   └── README.md                    # Hướng dẫn chạy giao diện
│
├── results/                         # Lưu kết quả thực nghiệm
│   ├── figures/                     # Biểu đồ, Confusion Matrix, PR Curve
│   ├── tables/                      # Bảng so sánh các mô hình
│   └── reports/                     # Báo cáo kết quả
│
├── docs/                            # Tài liệu dự án
│   ├── references/                  # Tài liệu và bài báo tham khảo
│   └── notes/                       # Ghi chú nghiên cứu
│
├── requirements.txt                 # Danh sách thư viện Python
├── README.md                        # Giới thiệu và hướng dẫn dự án
└── .gitignore                       # Các file không đưa lên GitHub