# FoodDelivery_TimePrediction_Clustering
# 📦 Ứng dụng các thuật toán Hồi Quy và K-Means trong dịch vụ giao đồ ăn

## 📌 Giới thiệu
Thời gian giao hàng là một yếu tố quan trọng ảnh hưởng trực tiếp đến mức độ hài lòng của khách hàng trong ngành dịch vụ giao đồ ăn. Bên cạnh đó, tài xế – mắt xích quan trọng trong chuỗi cung ứng – rất đa dạng về kinh nghiệm, kỹ năng và phong cách làm việc.  

Do đó, việc dự đoán thời gian giao hàng và phân nhóm tài xế theo đặc điểm tương đồng sẽ giúp doanh nghiệp:
- Tối ưu vận hành
- Cải thiện dịch vụ
- Phân bổ nguồn lực hợp lý

Trong dự án này:  

### Mô hình dự đoán thời gian giao hàng bằng các thuật toán hồi quy
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**

**Đánh giá mô hình** bằng các chỉ số:
- Mean Squared Error (MSE)
- R-squared (R²)

### Phân cụm tài xế bằng thuật toán K-Means
Thuật toán K-Means được áp dụng để phân cụm tài xế dựa trên hành vi và đặc điểm vận hành. Việc kết hợp cả hai mô hình này giúp doanh nghiệp:
- Dự đoán chính xác hơn thời gian giao hàng
- Nhận diện nhóm tài xế có hiệu suất tương đồng
- Xây dựng chính sách đào tạo, thưởng phạt và phân tuyến hợp lý
- Tối ưu hóa trải nghiệm khách hàng

**Dữ liệu sử dụng:** Food Delivery Dataset, thuộc lĩnh vực Logistics và dịch vụ giao đồ ăn, gồm 45.597 dòng và 20 cột.  

## 🎯 Mục tiêu dự án
- Phát triển mô hình dự đoán thời gian giao hàng chính xác và ổn định.
- Phân cụm tài xế giúp doanh nghiệp hiểu rõ đặc điểm từng nhóm tài xế.
- Tối ưu vận hành giao đồ ăn và nâng cao trải nghiệm khách hàng.

## 📁 Cấu trúc dự án

FoodDelivery_TimePrediction_Clustering/
├── app/ # Ứng dụng, mô hình đã huấn luyện, script deploy
│ ├── delivery_model.pkl
│ ├── delivery_scaler.pkl
│ └── predict_time_app.py
├── Data/ # Dữ liệu
│ ├── Food_Delivery_Dataset.csv
│ └── delivery_time_cleaned.csv
├── Driver_Cluster/ # Notebook về dự đoán thời gian
│ └── Delivery_time_prediction.ipynb
├── Time_Prediction/ # Notebook về phân cụm tài xế
│ └── DriverFeatures_Clustering.ipynb
├── Visualization/ # Dashboard / trực quan hóa
│ └── Food_delivery_dashboard.pbix
├── README.md
