# 🌸 Phân loại hoa Oxford-102 với HOG+SVM và VGG16 Transfer Learning  

![Link Data dữ liệu]https://www.kaggle.com/datasets/waseemalastal/the-oxford-flowers-102-dataset  

## 📌 Giới thiệu  

Dự án này thực hiện **bài toán phân loại 102 loài hoa** trong bộ dữ liệu **Oxford Flowers-102**.  
Chúng tôi xây dựng và so sánh hai phương pháp:  

1. **HOG + SVM** – Phương pháp truyền thống dựa trên trích xuất đặc trưng thủ công.  
2. **VGG16 Transfer Learning** – Phương pháp học sâu hiện đại, tận dụng mô hình đã huấn luyện sẵn trên ImageNet.  

Mục tiêu:  
- So sánh hiệu quả giữa phương pháp truyền thống và phương pháp học sâu.  
- Xây dựng pipeline huấn luyện → đánh giá → giao diện trực quan để dự đoán ảnh mới.  

---


## 🛠️ Công nghệ sử dụng
Ngôn ngữ: Python 3.9+

Thư viện:

numpy, pandas, matplotlib, seaborn

scikit-learn (cho HOG + SVM)

tensorflow / keras (cho VGG16 Transfer Learning)

gradio (xây dựng giao diện demo)

## 🌟 Điểm nổi bật của dự án
So sánh chi tiết thuật toán truyền thống vs học sâu.

Kết quả trực quan, minh họa bằng biểu đồ và confusion matrix.

Giao diện thân thiện, dễ sử dụng.

## 📖 Tài liệu tham khảo
Oxford Flowers Dataset: https://www.robots.ox.ac.uk/~vgg/data/flowers/102/

Simonyan & Zisserman, Very Deep Convolutional Networks for Large-Scale Image Recognition (VGG16).

Scikit-learn, TensorFlow, Keras official docs.

👨‍💻 Tác giả
Nhóm thực hiện: Đề tài 7 – Phân loại hoa Oxford-102

Gồm những thành viên: Trương Hữu Vinh, Lê Hưng Tâm, Nguyễn Hữu Bảo.

© 2025 NHÓM 17,Phân loại hoa Oxford-102 – NHẬP MÔN HỌC  – TRƯỜNG ĐẠI HỌC ĐẠI NAM
