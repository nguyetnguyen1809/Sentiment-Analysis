Đề tài " Phân tích cảm xúc khi mua hàng dựa vào các đánh giá của khách hàng trên ứng dụng Tiki" nhằm áp dụng các kỹ thuật xử lý ngôn ngữ tự nhiên và sử dụng các mô hình 
Machine Learning để tự động phân loại đánh giá sản phẩm thành hai nhóm: tích cực (positive) nếu văn bản thể hiện sự hài lòng, tán dương và tiêu cực (negative) nếu 
văn bản thể hiện sự thất vọng , phê phán. Qua đó cũng sẽ so sánh, đánh giá giữa cách hoạt động của ba mô hình để chọn ra được mô hình tối ưu để sử dụng cho đề tài này.  
Các bước thực hiện:
•	Thu thập dữ liệu từ sàn thương mại điện tử Tiki.
•	Xử lí dữ liệu và gán nhãn cảm xúc dựa trên “Rating”,áp dụng TF-IDF để biểu diễn văn bản,sử dụng SMOTE để cân bằng dữ liệu.
•	Huấn luyện mô hình phân tích sắc thái đánh giá sản phẩm trên Tiki bằng các mô hình Naive Bayes, Logistic Regression, SVM ,kèm theo tối ưu hóa tham số với GridSearchCV để đảm bảo hiệu suất của mô hình , sau đó sử dụng K-Fold Cross Validation để đánh giá mô hình một cách khách quan và ổn định bằng cách chia tập dữ liệu thành K phần (folds) và huấn luyện mô hình trên các phần con này để giảm thiểu sự phụ thuộc vào phân bổ ngẫu nhiên của dữ liệu. 
•	Đánh giá độ chính xác dựa trên các metrics accuracy, precision, recall, và F1-score, Confusion Matrix ( Ma trận nhầm lẫn).
•	Cuối cùng sử dụng Ensemble Learning để kết hợp nhiều mô hình phân loại khác nhau nhằm cải thiện hiệu quả dự đoán, giảm thiểu sai số và nâng cao độ chính xác tổng thể của mô hình, từ đó đưa ra dự đoán cho tập dữ liệu mới.
