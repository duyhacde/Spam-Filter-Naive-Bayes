### Tên đề tài 
Phân loại thư rác sử dụng mô hình Naive Bayes
### Mô tả
Sử dụng thuật toán Naive Bayes, mô hình sẽ xác định một email là thư rác hay không, qua đó phân loại một tập emails
### Ngôn ngữ: Python
### Cài đặt
Máy tính cần cài đặt môi trường và trình dịch đối với Python để chạy chương trình
Các thư viện cần có:
* pandas
* nltk
* numpy
* matplotlib
* collections

### Các bước xử lý:
Có thể chạy lần lượt các cell trong file SpamFilter.ipynb để có được kết quả từ đó đánh giá và so sánh độ hiệu quả của các cách biểu diễn dữ liệu (vocabulary) với nhau.

### Các lưu ý:
* Nếu thay đổi cấu trúc phân cấp các file, các thư mục thì file code sẽ không chạy được vì sử dụng đường dẫn cố định.
* Các cell trong file code đã được sắp xếp theo đúng thứ tự, nếu chạy cell không đúng thứ tự đó thì có thể code sẽ bị lỗi.
* Huấn luyện mô hình theo cách thông thường bằng các tập dữ liệu lớn như kaggle1.csv, kaggle3.csv,... sẽ khá tốn thời gian và tài nguyên tính toán. Cần hạn chế chạy lại vì kết quả các bước đã được hiển thị đầy đủ. Nếu phải chạy lại thì nên dùng colab để nhờ đến tài nguyên tính toán của google.
* Một số tập dữ liệu không có column label_text, nếu muốn code chạy được ta cần bỏ comment dòng tương tự như sau:<br>
sms_spam['label_text'] = sms_spam['label_num'].apply(lambda x: 'ham' if x == 0 else 'spam')



