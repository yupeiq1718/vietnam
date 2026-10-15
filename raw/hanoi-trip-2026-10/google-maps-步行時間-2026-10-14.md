# Google 地圖步行時間：Tru by Hilton Hanoi Station 出發

**這是原始紀錄，不要改。** 要更新就另存新檔。

## 怎麼取得

- 日期：2026-10-14
- 工具：Claude in Chrome，在 Google 地圖（繁體中文介面）開路線頁，交通方式選「步行」，沒有指定出發時間
- 方法：每個終點開一次 `https://www.google.com/maps/dir/?api=1&origin=Tru+by+Hilton+Hanoi+Station&destination=<查詢字串>&travelmode=walking`，看畫面左側的路線清單
- 數字是我從截圖（縮小到 0.6 倍）逐一抄下來的。沒有另存截圖
- 起點：畫面顯示 `Tru by Hilton Hanoi Station, 115 Trần Hưng Đạo`

## 結果

「解析到的終點」是 Google 把查詢字串對到哪個地點，畫面上被截斷的字尾用 … 表示。

| # | 查詢字串 | 解析到的終點 | 最快步行 | 其他路線（時間／距離／經過） |
|---|---|---|---|---|
| 1 | Moonlight Sky Bar 94 Ma May Hanoi | Moonlight Sky Bar, 94 Mã Mây… | 28 分，2.0 公里，經 P. Hàng Bông | 30 分／2.1 公里／Đ. Lê Duẩn；30 分／2.2 公里／P. Quán Sứ |
| 2 | Diamond Sky Bar 22 Ta Hien Hanoi | Diamond Sky Bar, 22 Tạ Hiện, Phố cổ Hà… | 26 分，1.9 公里，經 P. Hàng Bông | 28 分／2.0 公里／Đ. Lê Duẩn；28 分／2.0 公里／P. Quán Sứ |
| 3 | Skyline Hanoi Gia Ngu | Skyline Hanoi, 38 P. Gia Ngư, Phố cổ Hà N… | 25 分，1.8 公里，經 P. Hàng Bông | 27 分／1.9 公里／P. Quán Sứ；30 分／2.2 公里／Đ. Lê Duẩn |
| 4 | Terraco Sky Bar La Sinfonia del Rey Hang Dau Hanoi | Terraço Sky Bar, La Sinfonía Del Rey Hote… | 27 分，2.0 公里，經 P. Hàng Bông | 29 分／2.1 公里／P. Quán Sứ；32 分／2.3 公里／P. Tràng Thi |
| 5 | Majesty Sky Bar La Sinfonia Majesty Hanoi | Majesty Sky Bar, Rooftop, No 01 P. Cầu G… | 25 分，1.8 公里，經 P. Hàng Bông | 27 分／2.0 公里／P. Quán Sứ |
| 6 | La Nueva Boutique Hotel Hanoi 32 Lo Su | La Nueva Boutique Hotel Hanoi, 32 P. Lò… | 28 分，2.0 公里，經 P. Hàng Bông | 30 分／2.2 公里／P. Quán Sứ；34 分／2.4 公里／P. Tràng Thi |
| 7 | Lotte Hotel Hanoi 54 Lieu Giai Ba Dinh Hanoi Vietnam | Lotte Hotel Hanoi, 54 P. Liễu Giai, Giảng V… | 51 分，3.7 公里，經 P. Nguyễn Thái Học 和 P. Kim Mã | 53 分／3.8 公里／Trần Phú；54 分／3.9 公里／Cát Linh |
| 8 | Summit Bar Pan Pacific Hanoi | Summit Rooftop Bar, Khách sạn Pan Paci… | 44 分，3.2 公里，經 Nguyễn Trí Phương | 47 分／3.4 公里／Hoàng Diệu；48 分／3.4 公里／Thanh Niên |
| 9 | Hoan Kiem Lake Hanoi | 還劍湖 越南河內 Hoan Kiem（終點標記在湖面，靠近龜塔） | 29 分，2.1 公里，經 P. Tràng Thi | 29 分／2.1 公里／P. Hai Bà Trưng；31 分／2.2 公里／Lý Thường Kiệt |
| 10 | Hang Bac Street Hanoi | Phố Hàng Bạc, 59 P. Hàng Bạc, Phố cổ H… | 26 分，1.9 公里，經 P. Hàng Bông | 28 分／2.0 公里／Đ. Lê Duẩn；28 分／2.0 公里／P. Quán Sứ |

## 沒有採用的查詢

| 查詢字串 | 發生什麼事 |
|---|---|
| Top of Hanoi Lotte Hotel Hanoi | 沒有路線，地圖畫面跑到台北。改用第 7 列的查詢。第 7 列是 Lotte 飯店，不是 65 樓的酒吧本身 |
| Dong Kinh Nghia Thuc Square Hoan Kiem Hanoi | Google 把終點對到「河內老城區 100000越南 Hà Nội, Hoàn Kiếm」，不是廣場。畫面顯示 25 分、1.8 公里，不能當廣場的數字用 |

## 限制

- 步行時間是 Google 的估算，不含跨年夜的人潮與封路
- 終點是 Google 解析出的標記位置，不一定是入口
- 酒吧名稱只看到畫面上被截斷的部分，沒有逐一核對樓層
