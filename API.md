# API Docs
## Base
```
Endpoint: https://chiasenhac.vn/api/
Method: GET
```
## Lấy thông tin BXH
```
Endpoint: https://chiasenhac.vn/api/nhac-hot.html
Method: GET
Response:
- message: Tin nhắn
- code: HTTP Code
- data (Dữ liệu trả về):
    - dataBxh:
        - 3:
            - cat_name: Tên BXH
            - cat_url: URL/ID BXH
            - music (Thông tin bài hát):
                - music_downloads_today: Số lượt tải về hôm nay
                - music_id: ID bài hát
                - music_title_url: Tên URL bài hát
                - music_title: Tên bài hát
                - music_artist: Tác giả
                - music_artist_id: ID tác giả
```
## Lấy dữ liệu trang nhà
```
Endpoint: https://chiasenhac.vn/api/home
Method: GET
```
## Lấy toàn bộ chủ đề
```
Endpoint: https://chiasenhac.vn/api/chu-de/danh-sach-chu-de
Method: GET
Response:
- message: Tin nhắn
- code: HTTP Code
- data (Dữ liệu trả về):
    - key_url: ID chủ đề
    - caption: Tên chủ đề đầy đủ
    - label: Tên chủ đề rút gọn
    - image_url: URL ảnh chủ đề
- error: Lỗi (nếu có)
```
## Lấy một chủ để cụ thể
```
Endpoint: https://chiasenhac.vn/api/chu-de/%s
Method: GET<br>
Data:
- %s: Một trong những key_url được lấy từ response
```
## Đăng nhập
