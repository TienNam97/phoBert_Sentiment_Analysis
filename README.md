# phoBert_Sentiment_Analysis
## Data:
- Link data comment đánh giá trên sàn thương mại điện tử [vietnamese sentiment analysis](https://docs.google.com/spreadsheets/d/1XF2807xz5V1Ov1qstCxB6O4bOhQZSVmzHQRLTvNTBKI/edit?usp=sharing)

- Link data đánh giá môn học trường UIT [VSFC](https://drive.google.com/drive/folders/1XeUy3Fmrja70wKfGGfQ1UXogum0NlA77?usp=sharing)
## Model pretrained phoBert:

- Code để tải pretrained phoBert
```
wget https://public.vinai.io/PhoBERT_base_transformers.tar.gz
tar -xzvf PhoBERT_base_transformers.tar.gz
```
## Cách tổ chức dữ liệu:

- Tại My Drive, tạo một thư mục BERT và tạo một thư mục con SA trong thư mục BERT và lưu data vào đấy, bao gồm cả thư mục PhoBERT_base_transformers (đây là thư mục chưa những file để Load cũng như cấu hình phoBert)

- Hoặc các bạn có thể thay đổi đường dẫn tuỳ ý ở cell đầu
```
os.chdir('/content/drive/My Drive/BERT/SA')
```
 ## Lưu ý:
 - Ở file Sentiment Analysis - VSFC là load lại model đã lưu lại sau khi train ở file Sentiment Analysis with Fold - fixed bug nên các bạn chạy file Sentiment Analysis with Fold - fixed bug trước để lưu lại model sau khi train rồi mới chạy được file Sentiment Analysis - VSFC
 - Hoặc có thể tải model pretrained sau khi chạy trên Sentiment Analysis with Fold - fixed bug tại [đây](https://drive.google.com/drive/folders/1-4aRRtj1qlSoKbtQbSM-7RQ5qdYuvOQg?usp=sharing) (xài email org)
