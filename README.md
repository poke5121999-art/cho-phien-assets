# cho-phien-assets

Kho ảnh độ phân giải gốc của game Chợ Phiên (`games/bazaar` trong repo survivor-web-hub), đăng riêng trên GitHub Pages vì repo chính đã vượt 1 GB. Game luôn có bản webp 512 px làm nền; khi màn hình cần nét hơn (hoặc xem phóng to) nó tải bản trong kho này (`games/bazaar/js/view/hires.js`).

- `art/cards/*.webp`: art thẻ 1024x1024 (q82, bỏ alpha)
- `art/encounters/*.webp`: chân dung và nền quái, thương nhân, sự kiện ở cỡ nguồn (q82, `_bg` q78)
- Tên và đường dẫn trùng 1:1 với `games/bazaar/art/...`.
- Hiện có 1685 tệp, 129.5 MB.

## Cách sinh

Ở gốc repo survivor-web-hub (Python 3.8 + Pillow, sau `art.py` đã bóc PNG vào `D:azaar-refrt`):

    python -I games/bazaar/tools/hires.py

Chạy lại thì bỏ qua tệp không đổi. Sau đó commit và push repo này.
