# Bài: 5 quy tắc vàng và hàm trim

## Phần 1: Phân tích

bảng đang vi phạm 3 quy tắc:

- tiêu đề bị merge cell, mỗi cột phải có 1 ô tiêu đề riêng
- có hàng trống giữa bảng nên filter chỉ lọc được phần trên
- dữ liệu không đồng nhất, "hỏng " có dấu cách và "hỏng" bị tính là 2 giá trị khác nhau

## Phần 2: Hoàn thiện

1. thêm cột phụ cạnh cột trạng thái, gõ `=TRIM(D2)` rồi kéo xuống hết cột
2. copy cột phụ, paste values đè lại cột trạng thái rồi xóa cột phụ
3. unmerge ô tiêu đề, gõ lại tiêu đề cho từng cột
4. xóa các hàng trống giữa bảng
5. chọn cả vùng dữ liệu, bấm ctrl + shift + L

kết quả: cột trạng thái chỉ còn 1 nhóm "hỏng" và filter lọc đúng toàn bảng