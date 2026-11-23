# 6451071061_Lab1

Họ tên: Đinh Công Vinh Quang – MSSV: 6451071061 – Môn: Khai thác dữ liệu (LAB1)

## Đối chiếu file với mẫu báo cáo

### BÁO CÁO PHẦN 1
| Mục trong báo cáo | File | Nội dung |
|---|---|---|
| Bài 2 (Trang 15-17) | Bai1 | Titanic: nhập dữ liệu, thống kê cơ bản |
| | Bai2 | Titanic: 5 thuộc tính nhiều giá trị rỗng nhất |
| | Bai3 | Titanic: tuổi, giới tính, sống sót |
| | Bai4 | Titanic: cổng lên tàu, loại vé, sống sót |
| | Bai5 | Titanic: số người đi cùng |
| | Bai6 | Titanic: tiền xử lý dữ liệu thiếu |
| | Bai7 | Titanic: biến đổi thuộc tính |
| | Bai8 | Titanic: tạo thuộc tính mới (age_class, fare_per_person) |
| Bài 2 (Trang 28) | Bai9 | Bank marketing: khảo sát + tiền xử lý bảng mẫu 16 dòng |
| Bài 2 (Trang 30) | Bai10 | tb_tracking.xlsx (Bài tập thêm VI.2, yêu cầu a-d) |

### BÁO CÁO PHẦN 2
| Mục trong báo cáo | File | Nội dung |
|---|---|---|
| Bài 2 (Trang 37, 38) | Bai11 | Online Retail: bước 1-8 (đọc, làm sạch, ma trận hóa đơn) |
| | Bai12 | Online Retail: bước 9-11 (Apriori, luật, scatter plot) |
| | Bai13 | Online Retail: bước 12 (FP-Growth, so sánh với Apriori) |
| Bài 5a (Trang 45) | Bai14 | Germany, min_sup 5%, min_conf 50% |
| Bài 6 (Trang 45) | Bai15 | Groceries: Apriori vs FP-Growth, min_sup 0.01%-0.1% |

Không có notebook cho Bài tập thêm VI.1 (vnexpress) vì không có file dữ liệu và mẫu báo cáo không có mục này.

## Chuẩn bị chạy
Đặt dữ liệu cùng thư mục với notebook: `titanic.csv`, `tb_tracking.xlsx`, `Online_Retail.xlsx` (đổi tên có dấu gạch dưới), `groceries.csv`.
Chạy trên Google Colab: upload notebook + dữ liệu, Runtime -> Run all (nếu thiếu mlxtend: thêm ô `!pip install mlxtend`).

## Đẩy lên GitHub (repo public tên 6451071061_Lab1)
Tạo repo trên github.com rồi kéo thả các file .ipynb (và README.md) vào trang repo, hoặc dùng git:
```
git init && git add *.ipynb README.md && git commit -m "LAB1 - 6451071061"
git branch -M main
git remote add origin https://github.com/<ten-github>/6451071061_Lab1.git
git push -u origin main
```

## Ghi chú
- Bai15 dùng `max_len=3` (và `low_memory=True`) vì min_sup 0.01% khiến số tổ hợp bùng nổ.
- Bai10: file có 4 dòng cuối không phải dữ liệu đo (1 dòng trống + 3 dòng min/max/mean) nên đã loại bỏ.
