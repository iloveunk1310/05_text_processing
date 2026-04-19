1. Tổng quan
Notebook này trình bày một quy trình xử lý ngôn ngữ tự nhiên (NLP) chi tiết trên bộ dữ liệu 20newsgroups, tập trung vào việc so sánh hiệu quả của các kỹ thuật tiền xử lý và vector hóa khác nhau. Các nội dung chính bao gồm:

* Phân tích Thống kê (EDA): Khám phá đặc điểm độ dài văn bản, phân phối nhãn, kiểm định Mann-Whitney U và kiểm chứng định luật Zipf.

* Pipeline Tiền xử lý: Làm sạch văn bản (loại bỏ HTML, URL, ký tự đặc biệt), so sánh các chiến lược Tokenization (Word, Char, BPE) và loại bỏ Stop words.

* Chuẩn hóa văn bản: So sánh thực nghiệm giữa các kỹ thuật Stemming (Porter, Snowball) và Lemmatization về tốc độ cũng như tác động đến độ chính xác của mô hình phân loại.

* Vector hóa & Không gian đặc trưng: Thực hiện BoW, TF-IDF và Word2Vec; trực quan hóa bằng t-SNE và đánh giá bằng chỉ số Silhouette.

* Mô hình Ngữ nghĩa: Sử dụng Sentence Transformer (SBERT) để so sánh hiệu suất phân loại và phân cụm với phương pháp TF-IDF truyền thống.

2. Cách chạy

Yêu cầu cài đặt
**Đảm bảo bạn đã cài đặt các thư viện Python sau**:

numpy, pandas

scikit-learn

wordcloud

spacy, nltk, tokenizers

scipy, matplotlib, seaborn

gensim

sentence-transformers

**Các bước thực hiện**

* Mở Notebook: Sử dụng Jupyter Notebook hoặc Google Colab để mở file 05_text_preprocessing.ipynb.

* Tải dữ liệu: Notebook sử dụng thư viện sklearn.datasets để tự động tải bộ dữ liệu 20newsgroups. Yêu cầu có kết nối internet trong lần chạy đầu tiên.

* Chạy tuần tự: Thực thi các cell từ trên xuống dưới. Các bước tiền xử lý đã được đóng gói thành các hàm và pipeline để dễ dàng theo dõi kết quả thay đổi của dữ liệu.

* Quan sát kết quả: Các biểu đồ trực quan (t-SNE, Word Cloud) và bảng so sánh hiệu suất (Accuracy, F1-score) sẽ được hiển thị trực tiếp sau mỗi bước thực nghiệm
