# Data Science & AI Projects Portfolio (TieuLuanTotNghiep_AI)

Chào mừng bạn đến với repository của mình! Đây là nơi lưu trữ các dự án học thuật và cá nhân tập trung vào lĩnh vực **Khoa học dữ liệu (Data Science)**, **Học máy (Machine Learning)**, và **Học sâu (Deep Learning)**. 

Repository này bao gồm 2 dự án chính: Xử lý ảnh y tế (Medical Image Classification) và Khai phá dữ liệu (Data Mining).

---

## Cấu trúc Repository

Repo chứa các Jupyter Notebooks ứng với từng phần của dự án:

1. **Cardiomegaly Disease Classifier (Phân loại bệnh lý tim to từ ảnh X-quang)**
   - `Cardiomegaly_Disease_Classifier_RF_SVM_KNN.ipynb`: Huấn luyện và đánh giá bằng các thuật toán Machine Learning truyền thống.
   - `cardiomegaly-disease-classifier-efficientnet.ipynb`: Huấn luyện bằng mô hình Deep Learning (CNN - EfficientNet) trên môi trường Kaggle Notebook.
   - `Cardiomegaly_Disease_Classifier.ipynb`: Notebook tổng hợp các bước tiền xử lý và xây dựng mô hình.
   - Link File Doc tiểu luận: https://ap.wps.com/l/cbTaqgjaxDcqr3tC
2. **Data Mining - Adult Dataset (Khai phá dữ liệu & Dự đoán thu nhập)**
   - `ProjectDM.ipynb` (hoặc `ProjectDataMining.ipynb`): Khám phá dữ liệu (EDA), tiền xử lý và áp dụng các thuật toán phân lớp để dự đoán mức thu nhập.

---

## Công nghệ & Thư viện sử dụng

- **Ngôn ngữ:** Python 
- **Xử lý dữ liệu & Tính toán:** Pandas, NumPy
- **Trực quan hóa:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn (Random Forest, SVM, KNN, Naive Bayes, Multi-layer Perceptron)
- **Deep Learning / Computer Vision:** TensorFlow, Keras, OpenCV (cv2)
- **Môi trường:** Jupyter Notebook, Google Colab, Kaggle Notebook (Sử dụng GPU)

---

## Chi tiết các dự án

1. Phân loại bệnh lý cơ tim (Cardiomegaly Disease Classifier)
Dự án này tập trung vào việc tự động hóa quá trình nhận diện bệnh lý tim to (Cardiomegaly) từ hình ảnh X-quang ngực. Điểm nổi bật của dự án là sự **so sánh toàn diện giữa Machine Learning và Deep Learning**.

Tiền xử lý & Data Augmentation: Xử lý ảnh với OpenCV (resize 224x224) và tăng cường dữ liệu bằng `ImageDataGenerator` để tránh Overfitting.
- Cách tiếp cận Machine Learning: Sử dụng Random Forest, SVM, và KNN kết hợp với `GridSearchCV` để tối ưu hóa siêu tham số (Hyperparameter tuning). Kỹ thuật làm phẳng ảnh (flatten) được áp dụng để trích xuất đặc trưng.
- Cách tiếp cận Deep Learning (CNN):Xây dựng mô hình sử dụng kiến trúc **EfficientNet**. Đây là một mạng nơ-ron tích chập (CNN) tiên tiến, giúp tự động học và trích xuất các đặc trưng không gian phức tạp của hình ảnh y tế hiệu quả hơn nhiều so với việc làm phẳng ảnh thủ công ở các thuật toán ML truyền thống.
- Việc huấn luyện mô hình CNN được thực hiện trên **Kaggle Notebook** nhằm tận dụng tài nguyên GPU, giảm thiểu thời gian training.

### 2. Khai phá dữ liệu và dự đoán thu nhập (Adult Dataset)
Mục tiêu của dự án là dự đoán xem một cá nhân có thu nhập trên 50K/năm hay không dựa trên các đặc trưng nhân khẩu học (độ tuổi, giáo dục, nghề nghiệp,...).

* **Exploratory Data Analysis (EDA):** Trực quan hóa phân bố dữ liệu và tìm ra mối tương quan giữa các đặc trưng thông qua biểu đồ của Seaborn (`histplot`, `boxplot`, `countplot`).
* **Tiền xử lý:** Chuẩn hóa biến số bằng `StandardScaler`, xử lý các biến phân loại bằng `LabelEncoder` và `OneHotEncoder` (`pd.get_dummies`).
* **Mô hình hóa:** Huấn luyện và đánh giá đa mô hình bao gồm Random Forest, Gaussian Naive Bayes, và MLPClassifier. Các chỉ số như Accuracy, Precision, Recall, F1-Score được tính toán và vẽ biểu đồ so sánh để chọn ra mô hình tối ưu nhất.

---
Hướng dẫn cài đặt và sử dụng

1. Clone repository này về máy:
   ```bash
   git clone [https://github.com/your-username/tieuluantotnghiep_ai.git](https://github.com/your-username/tieuluantotnghiep_ai.git)
   cd tieuluantotnghiep_ai
2. Cài đặt các thư viện cần thiết:
Đảm bảo bạn đã cài đặt Python. Cài đặt các thư viện thông qua pip:
pip install pandas numpy scikit-learn tensorflow opencv-python matplotlib seaborn
3. Chạy các Notebooks:
Bạn có thể mở các file .ipynb bằng Jupyter Notebook hoặc Jupyter Lab
Hoặc upload các file này lên Google Colab / Kaggle để chạy trực tiếp trên trình duyệt nếu máy tính cá nhân không có GPU.
