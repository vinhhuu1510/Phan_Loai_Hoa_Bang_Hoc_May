# 🌸 Phân loại hoa Oxford-102 với HOG+SVM và VGG16 Transfer Learning  

![Oxford Flowers](https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/Flowers_in_the_garden.JPG/640px-Flowers_in_the_garden.JPG)  

## 📌 Giới thiệu  

Dự án này thực hiện **bài toán phân loại 102 loài hoa** trong bộ dữ liệu **Oxford Flowers-102**.  
Chúng tôi xây dựng và so sánh hai phương pháp:  

1. **HOG + SVM** – Phương pháp truyền thống dựa trên trích xuất đặc trưng thủ công.  
2. **VGG16 Transfer Learning** – Phương pháp học sâu hiện đại, tận dụng mô hình đã huấn luyện sẵn trên ImageNet.  

Mục tiêu:  
- So sánh hiệu quả giữa phương pháp truyền thống và phương pháp học sâu.  
- Xây dựng pipeline huấn luyện → đánh giá → giao diện trực quan để dự đoán ảnh mới.  

---

## 📂 Cấu trúc thư mục  

```bash
├── data/                  # Bộ dữ liệu Oxford-102 (link tải bên dưới)
├── notebooks/             # Các notebook Jupyter demo
│   ├── hog_svm.ipynb      # Thực nghiệm với HOG + SVM
│   ├── vgg16_transfer.ipynb  # Thực nghiệm với VGG16 Transfer Learning
├── src/                   # Code chính
│   ├── data_loader.py     # Hàm load & tiền xử lý dữ liệu
│   ├── hog_svm.py         # Huấn luyện + đánh giá HOG+SVM
│   ├── vgg16_model.py     # Xây dựng mô hình VGG16 Transfer Learning
│   ├── gui.py             # Giao diện demo bằng Gradio
├── requirements.txt       # Thư viện cần thiết
├── README.md              # File mô tả (tài liệu này)
└── results/               # Lưu kết quả, confusion matrix, model
📥 Cài đặt
1. Clone repo
bash
Sao chép mã
git clone https://github.com/<username>/Oxford102-Flower-Classification.git
cd Oxford102-Flower-Classification
2. Cài môi trường
Khuyên dùng conda hoặc venv.

bash
Sao chép mã
pip install -r requirements.txt
3. Tải dữ liệu Oxford-102
Link chính thức: Oxford-102 Flowers Dataset

Hoặc tải nhanh qua Kaggle:

bash
Sao chép mã
kaggle datasets download -d nikhil25/oxford-102-flower-png
unzip oxford-102-flower-png.zip -d data/
🚀 Chạy thử
1. Huấn luyện HOG + SVM
bash
Sao chép mã
python src/hog_svm.py
2. Huấn luyện VGG16 Transfer Learning
bash
Sao chép mã
python src/vgg16_model.py
3. Chạy giao diện demo (Gradio)
bash
Sao chép mã
python src/gui.py
Giao diện sẽ mở tại: http://127.0.0.1:7860

📊 Kết quả
Phương pháp	Accuracy (%)	Training time	Ghi chú
HOG + SVM	~45–55%	Trung bình	Baseline, nhạy cảm với ánh sáng/rotate
VGG16 Transfer Learn	~85–90%	Nhanh (nhờ fine-tuning)	Chính xác cao, ổn định

Confusion matrix và các biểu đồ được lưu trong thư mục results/.

Ví dụ kết quả VGG16:


🛠️ Công nghệ sử dụng
Ngôn ngữ: Python 3.9+

Thư viện:

numpy, pandas, matplotlib, seaborn

scikit-learn (cho HOG + SVM)

tensorflow / keras (cho VGG16 Transfer Learning)

gradio (xây dựng giao diện demo)

🌟 Điểm nổi bật của dự án
So sánh chi tiết thuật toán truyền thống vs học sâu.

Kết quả trực quan, minh họa bằng biểu đồ và confusion matrix.

Giao diện thân thiện, dễ sử dụng.

📖 Tài liệu tham khảo
Oxford Flowers Dataset: https://www.robots.ox.ac.uk/~vgg/data/flowers/102/

Simonyan & Zisserman, Very Deep Convolutional Networks for Large-Scale Image Recognition (VGG16).

Scikit-learn, TensorFlow, Keras official docs.

👨‍💻 Tác giả
Nhóm thực hiện: Đề tài 7 – Phân loại hoa Oxford-102

Thành viên: (Điền tên các thành viên nhóm)

Liên hệ: <email của bạn nếu muốn>
