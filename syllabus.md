# **Đề Cương Đồ Án: Chẩn Đoán Bệnh Cây Trồng Dựa Trên Ảnh Lá Cây**

## **1. Giới thiệu**
- **Bài toán**: 
  - Nông nghiệp là ngành kinh tế quan trọng tại Việt Nam, nhưng các bệnh trên cây trồng gây thiệt hại lớn về năng suất và chất lượng. Theo báo cáo của **Tổ chức Lương thực và Nông nghiệp Liên Hợp Quốc (FAO)**, mỗi năm, khoảng **20-40% sản lượng cây trồng toàn cầu** bị mất do sâu bệnh và dịch bệnh cây trồng. 
  - Tại Việt Nam, theo **Bộ Nông nghiệp và Phát triển Nông thôn (MARD)**, bệnh đạo ôn trên lúa gây thiệt hại từ **10-15% năng suất** ở các vùng Đồng bằng sông Cửu Long và Đồng bằng sông Hồng. Bệnh gỉ sắt trên cà phê có thể làm giảm năng suất tới **30%** nếu không được phát hiện và xử lý kịp thời.
  - Việc phát hiện sớm và chính xác các bệnh trên cây trồng là một thách thức lớn đối với nông dân.
  - Đề tài này tập trung vào việc xây dựng một hệ thống sử dụng **Deep Learning** để chẩn đoán bệnh trên lá cây thông qua hình ảnh, giúp nông dân phát hiện bệnh nhanh chóng và đưa ra biện pháp xử lý kịp thời.
- **Phạm vi**:
  - Chỉ tập trung vào các loại cây phổ biến tại Việt Nam như: lúa, cà phê, tiêu, thanh long, xoài.
- **Mục tiêu**:
  - Xây dựng mô hình Deep Learning để phân loại bệnh trên lá cây.
  - Tạo một giao diện web demo để người dùng tải ảnh lá cây và nhận kết quả chẩn đoán.
  - Viết báo cáo bằng tiếng Anh dài 3-4 trang.

---

## **2. Mục tiêu**
- **Mục tiêu chính**:
  - Phát triển một hệ thống tự động chẩn đoán bệnh cây trồng dựa trên ảnh lá cây.
- **Mục tiêu cụ thể**:
  1. Thu thập và tiền xử lý dữ liệu ảnh lá cây từ các nguồn công khai và thực địa.
  2. Huấn luyện mô hình Deep Learning để phân loại bệnh trên lá cây.
  3. Đánh giá hiệu suất mô hình bằng các chỉ số như Accuracy, Precision, Recall, F1-score.
  4. Xây dựng một giao diện web demo để triển khai mô hình.
  5. Viết báo cáo và trình bày kết quả.

---

## **3. Nội dung và phương pháp**
### **3.1. Thu thập và tiền xử lý dữ liệu**
- **Nguồn dữ liệu**:
  - Sử dụng các bộ dữ liệu công khai như [PlantVillage Dataset](https://www.kaggle.com/emmarex/plantdisease).
  - Tự thu thập ảnh lá cây từ thực địa tại Việt Nam (lúa, cà phê, tiêu, thanh long, xoài).
- **Tiền xử lý dữ liệu**:
  - Loại bỏ ảnh không liên quan hoặc chất lượng kém.
  - Gắn nhãn (label) cho từng ảnh, ví dụ: "Lúa - Bệnh đạo ôn", "Cà phê - Bệnh gỉ sắt".
  - Chia dữ liệu thành các tập: huấn luyện (training), kiểm tra (testing), và xác thực (validation).

### **3.2. Huấn luyện mô hình Deep Learning**
- **Mô hình**:
  - Sử dụng các mô hình phổ biến như ResNet, MobileNet, hoặc EfficientNet.
  - Áp dụng Transfer Learning để tận dụng các mô hình đã được huấn luyện trước.
- **Thư viện**:
  - TensorFlow, Keras, hoặc PyTorch.
- **Quy trình**:
  1. Chia dữ liệu thành các tập huấn luyện, kiểm tra và xác thực.
  2. Huấn luyện mô hình trên tập dữ liệu huấn luyện.
  3. Tinh chỉnh tham số (hyperparameters) để tối ưu hóa hiệu suất.

### **3.3. Đánh giá thực nghiệm**
- **Chỉ số đánh giá**:
  - Accuracy, Precision, Recall, F1-score.
- **So sánh**:
  - So sánh hiệu suất giữa các mô hình khác nhau để chọn mô hình tốt nhất.

### **3.4. Xây dựng Web Demo**
- **Công cụ**:
  - Flask hoặc Django để xây dựng backend.
  - HTML/CSS/JavaScript hoặc Streamlit để xây dựng giao diện.
- **Chức năng**:
  - Cho phép người dùng tải ảnh lá cây lên.
  - Hiển thị kết quả chẩn đoán (tên bệnh, mức độ nghiêm trọng).
  - Đưa ra gợi ý xử lý cơ bản.

---

## **4. Kết quả dự kiến**
- **Kết quả mô hình**:
  - Mô hình Deep Learning đạt độ chính xác trên 90% trong việc phân loại bệnh trên lá cây.
- **Web demo**:
  - Một giao diện web đơn giản, cho phép người dùng tải ảnh lá cây và nhận kết quả chẩn đoán.
- **Báo cáo**:
  - Báo cáo bằng tiếng Anh dài 3-4 trang, bao gồm các phần: Introduction, Related Work, Methodology, Results and Discussion, Conclusion.

---

## **5. Kế hoạch thực hiện**
1. **Tuần 1-2**: Thu thập và tiền xử lý dữ liệu.
2. **Tuần 3-4**: Huấn luyện và đánh giá mô hình Deep Learning.
3. **Tuần 5**: Xây dựng giao diện web demo.
4. **Tuần 6**: Viết báo cáo và chuẩn bị bài thuyết trình.

---

## **6. Tài liệu tham khảo**
- [PlantVillage Dataset](https://www.kaggle.com/emmarex/plantdisease)
- [Transfer Learning with TensorFlow](https://www.tensorflow.org/tutorials/images/transfer_learning)
- [Flask Documentation](https://flask.palletsprojects.com/)
- [Streamlit Documentation](https://docs.streamlit.io/)
- FAO: [Plant Pests and Diseases](https://www.fao.org/news/story/en/item/1187738/icode/)
- MARD: [Báo cáo về bệnh cây trồng tại Việt Nam](http://www.mard.gov.vn)