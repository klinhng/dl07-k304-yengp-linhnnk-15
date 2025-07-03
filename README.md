# dl07-k304-yengp-linhnnk-15

# Các thao tác trên app tạo từ streamlit

## 1. Sidebar (Thanh bên trái)
- **Logo & tên app:** Hiển thị logo và tiêu đề "IT Recommendation System".
- **Menu điều hướng:**  
  Có 3 lựa chọn:
  - **Business Problem:** Phân tích nghiệp vụ, mô tả bài toán.
  - **Build Project:** Quy trình xây dựng mô hình, các bước phân tích.
  - **New Prediction:** Phân tích chi tiết từng công ty từ dữ liệu review.
- **Thông tin nhóm thực hiện:** Hiển thị tên lớp, tên học viên, email.

---

## 2. Tab "Business Problem"
- **Giới thiệu bài toán:**  
  - Trình bày mục tiêu ứng dụng: phân tích cảm xúc review, phân cụm thông tin đánh giá doanh nghiệp IT.
  - Nêu ý nghĩa thực tiễn cho doanh nghiệp và ứng viên.
- **Phân tích cảm xúc:**  
  - Giải thích mục tiêu, nguồn dữ liệu, lợi ích của việc xác định cảm xúc review.
- **Phân cụm thông tin:**  
  - Giải thích mục tiêu, nguồn dữ liệu, lợi ích của việc phân nhóm review.
- **Thông báo:**  
  - Gợi ý người dùng trải nghiệm các tính năng ở tab tiếp theo.

---

## 3. Tab "Build Project"
Chia thành nhiều tab nhỏ mô tả quy trình phân tích dữ liệu:

- **Business Understanding:**  
  - Trình bày mục tiêu phân tích cảm xúc và phân cụm.
- **Data Understanding:**  
  - Mô tả các file dữ liệu sử dụng: Overview_Companies, Overview_Reviews, Reviews.
- **Data Preparation:**  
  - Trình bày các bước tiền xử lý văn bản: xóa stopword, chuẩn hóa, tokenize, vector hóa.
- **Modeling:**  
  - Liệt kê các mô hình đã thử nghiệm cho sentiment (XGBoost, Logistic Regression, v.v.) và clustering (KMeans, LDA...).
- **Evaluation:**  
  - Nêu các tiêu chí đánh giá mô hình: accuracy, F1, silhouette score, trực quan hóa.
- **Deployment:**  
  - Mô tả các tính năng dashboard: wordcloud, từ khóa, cụm, đề xuất cải thiện.

---

## 4. Tab "New Prediction" (Phân tích công ty cụ thể)
Đây là nơi người dùng tương tác trực tiếp với dữ liệu review:

### a. Chọn công ty để phân tích
- Người dùng chọn tên công ty từ danh sách.
- Nếu có cột ngày review, có thể lọc theo khoảng thời gian.

### b. Tổng quan đánh giá
- Hiển thị tổng số review, điểm trung bình.
- Vẽ biểu đồ phân bố cảm xúc (positive, negative, neutral).

### c. Nhận xét tiêu biểu
- Chọn loại cảm xúc (positive/negative/neutral) để xem danh sách review tương ứng.
- Hiển thị bảng các review nổi bật theo cảm xúc đã chọn.

### d. WordCloud cảm xúc
- Tạo wordcloud cho các review tích cực và tiêu cực, giúp nhìn nhanh các từ khóa nổi bật.

### e. Phân cụm thông tin đánh giá
- Nếu dữ liệu có cột cluster/x/y, vẽ biểu đồ phân cụm các review.
- Hiển thị wordcloud từ khóa chính cho từng cụm.
- Thống kê số review trong mỗi cụm.

### f. Đề xuất cải thiện cho công ty
- Nếu số review tiêu cực nhiều hơn tích cực, cảnh báo công ty nên cải thiện.
- Hiển thị danh sách các góp ý cải thiện tiêu biểu từ review tiêu cực.

---

**Tóm lại:**  
App này cho phép người dùng khám phá tổng quan bài toán, hiểu quy trình phân tích, và đặc biệt là phân tích chi tiết từng công ty IT dựa trên dữ liệu review thực tế, với các biểu đồ, wordcloud, phân cụm và đề xuất cải thiện rõ ràng, trực quan.

