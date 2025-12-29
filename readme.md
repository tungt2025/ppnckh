# Hướng Dẫn Thực Hiện Đồ Án

## 1. Yêu Cầu Cần Đáp Ứng

### Tên Đề Tài
- Tên đề tài bắt buộc phải có Tiếng Việt, Tiếng Anh là tùy chọn.
- Tên đề tài cần ngắn gọn, đủ ý và mang tính khái quát.

### Đề Cương (Proposal)
- Đề cương là phác thảo những gì dự định làm, bao gồm:
  - Mục tiêu
  - Phương pháp
  - Kết quả dự kiến
- Đề cương cần ngắn gọn, logic và kết nối chặt chẽ giữa các phần.

### Nội Dung Đề Cương
1. **Giới thiệu**:
   - Mô tả bài toán/vấn đề cần giải quyết.
   - Mô tả input và output.
   - Lý do chọn đề tài, khả năng ứng dụng thực tế, tính thời sự.
2. **Mục tiêu**:
   - Cụ thể, rõ ràng, tránh mơ hồ.
3. **Nội dung và phương pháp**:
   - Viết chi tiết các bước thực hiện để đạt mục tiêu.
   - Ví dụ: cài đặt crawler, tạo danh sách các site để crawl.
4. **Kết quả dự kiến**:
   - Định lượng, so sánh, mô tả chi tiết những gì sẽ được hiện thực.

### Văn Phong
- Tránh dùng đại từ nhân xưng như "Em".
- Ưu tiên dùng thể bị động hoặc "Chúng tôi".

### Đánh Giá Đồ Án
- Tiêu chí đánh giá:
  - Đúng phương pháp luận (70%).
  - Kết quả - mức độ hoàn chỉnh, khả thi (30%).
- Nội dung đánh giá:
  - Computational Thinking - 4 Pillars.
  - Writing: key sentence, coherence, connecting, reference formatting.
  - Content: tên đề tài, giới thiệu, mục tiêu, nội dung, kết quả dự kiến.

### Tài Liệu Tham Khảo
- Tài liệu tham khảo phải được ghi đúng cách, bao gồm:
  - Tên tác giả
  - Tên công trình
  - Nơi xuất bản/công bố
  - Năm công bố
- Định dạng tài liệu tham khảo theo chuẩn DBLP. Ví dụ: Joseph Redmon, Ali Farhadi: YOLO9000: Better, Faster, Stronger. CVPR 2017: 6517-6525

---

## 2. Phương Pháp Thực Hiện Đồ Án

1. **Chọn Chủ Đề**:
   - Chủ đề liên quan đến các lĩnh vực ứng dụng như:
     - **Education**: Ví dụ, phân tích hành vi học tập của học sinh.
     - **Bioinformatics**: Ví dụ, khai thác dữ liệu gen để dự đoán bệnh.
     - **Agriculture**: Ví dụ, dự đoán năng suất cây trồng dựa trên dữ liệu thời tiết.
     - **Environmental Sustainability**: Ví dụ, phân tích dữ liệu khí hậu để dự đoán ô nhiễm.
     - **Geographic**: Ví dụ, khai thác dữ liệu GPS để phân tích hành vi di chuyển.
   - Tiêu chí chọn bài báo:
     - Phù hợp với sở thích.
     - Có dataset công khai.
     - Có source code trên GitHub.
     - Có demo minh họa trên YouTube.

2. **Thu Thập và Tiền Xử Lý Dữ Liệu**:
   - **Data collection**:
     - Tìm kiếm các bộ dữ liệu công khai từ Kaggle, UCI Machine Learning Repository, hoặc các nguồn mở khác.
     - Nếu không có sẵn, tự thu thập dữ liệu từ API, web scraping, hoặc cảm biến.
   - **Data preprocessing**:
     - Làm sạch dữ liệu: Loại bỏ dữ liệu trùng lặp, xử lý giá trị thiếu.
     - Chuẩn hóa dữ liệu: Chuyển đổi dữ liệu về định dạng phù hợp (ví dụ: chuẩn hóa giá trị số).
     - Trích xuất đặc trưng: Chọn các thuộc tính quan trọng để sử dụng trong mô hình.

3. **Chọn Kỹ Thuật Khai Thác Dữ Liệu**:
   - **Itemset Mining**: Tìm các tập hợp mục phổ biến trong dữ liệu (ví dụ: phân tích giỏ hàng).
   - **Sequential Mining**: Phân tích các chuỗi sự kiện để tìm mẫu tuần tự (ví dụ: hành vi người dùng theo thời gian).
   - **Trajectory Data Mining**: Phân tích dữ liệu quỹ đạo (ví dụ: dữ liệu GPS, hành trình di chuyển).

4. **Áp Dụng Machine Learning/Deep Learning**:
   - Chọn mô hình phù hợp:
     - **Machine Learning**: SVM, Random Forest, Decision Tree, KNN, etc.
     - **Deep Learning**: CNN, RNN, LSTM, Transformer, etc.
   - Huấn luyện mô hình:
     - Chia dữ liệu thành tập huấn luyện và kiểm tra.
     - Sử dụng thư viện như Scikit-learn, TensorFlow, hoặc PyTorch để triển khai mô hình.
   - Tinh chỉnh tham số để tối ưu hóa hiệu suất.

5. **Đánh Giá Thực Nghiệm**:
   - **Experimental Evaluation**:
     - Sử dụng các chỉ số đánh giá như Accuracy, Precision, Recall, F1-score, hoặc RMSE.
     - So sánh hiệu suất giữa các mô hình hoặc phương pháp khác nhau.
     - Trình bày kết quả dưới dạng bảng, biểu đồ để dễ hiểu.

6. **Xây Dựng Web Demo**:
   - Sử dụng các công cụ như Flask, Django (Python) hoặc Node.js để xây dựng giao diện web.
   - Triển khai mô hình đã huấn luyện để chạy trên web.
   - Tạo các tính năng như tải dữ liệu, chạy mô hình, hiển thị kết quả.

7. **Viết Báo Cáo Bằng Tiếng Anh**:
   - Báo cáo dài 3-4 trang, bao gồm các phần:
     1. **Introduction**: Giới thiệu chủ đề, bài toán, và mục tiêu.
     2. **Related Work**: Tóm tắt các nghiên cứu liên quan.
     3. **Methodology**: Mô tả dữ liệu, phương pháp khai thác, và mô hình.
     4. **Results and Discussion**: Trình bày kết quả thực nghiệm và phân tích.
     5. **Conclusion**: Kết luận và hướng phát triển trong tương lai.
   - Đảm bảo báo cáo đúng chuẩn, có tài liệu tham khảo theo định dạng DBLP.

---

## 3. Các Bước Thực Hiện

1. **Chuẩn Bị**:
   - Tìm kiếm và chọn bài báo phù hợp.
   - Thu thập tài liệu tham khảo và các link liên quan.

2. **Xây Dựng Đề Cương**:
   - Viết phần giới thiệu, mục tiêu, nội dung và phương pháp, kết quả dự kiến.
   - Đảm bảo tính logic và kết nối giữa các phần.

3. **Thực Hiện Đồ Án**:
   - Cài đặt các thuật toán, xây dựng hệ thống theo nội dung đề cương.
   - Thu thập và xử lý dữ liệu.

4. **Viết Báo Cáo**:
   - Tổng hợp kết quả, so sánh và đánh giá.
   - Đảm bảo báo cáo đúng chuẩn, đầy đủ các phần.

5. **Trình Bày**:
   - Chuẩn bị slide trình bày theo cấu trúc WHAT, WHY, WHERE, WHO.
   - Tránh các lỗi phổ biến trong trình bày PowerPoint.

---

## 4. Tham Khảo
- [Những lỗi phổ biến trong trình bày PowerPoint](https://nguyenvantuan830970966.wordpress.com/2021/04/05/nhung-loi-pho-bien-trong-trinh-bay-bang-powerpoint/?authuser=1)
- [Kỹ thuật viết 5-sentence paragraph](https://ielts-simon.com/ielts-help-and-english-pr/2011/10/ielts-writing-5-sentence-paragraphs.html?authuser=1)
- [Mẫu trình bày tham khảo](https://www.youtube.com/watch?v=ca0Xi1Y2c8o&authuser=1)
- [Idea Hexagon](https://www.youtube.com/watch?v=fYnJPtEJj4s&authuser=1)