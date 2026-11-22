# Tự đánh giá — Phạm Trọng Hiện - 2A202603218 · G09

## 1. Tự rà soát 4 cảnh

Bốn ca dưới đây tổng hợp từ ghi chú trong `disagreement_log.csv`. Cột “Loại lỗi” ghi nội dung cần rà. `ok` là ca mình giữ nguyên theo ghi chú đã ghi trong log.

| Ảnh         | Đối tượng                | Loại lỗi    | Ghi chú                                                                                                      | Đã sửa?    |
| ----------- | ------------------------ | ----------- | ------------------------------------------------------------------------------------------------------------ | ---------- |
| S04_rgb.png | Dây an toàn của người    | `ok`        | `not_worn` vì trên ảnh RGB thấy rõ người không đeo dây. Nếu vùng dây không nhìn rõ thì dùng `unknown`.       | Giữ nguyên |
| S08_ir.png  | Vị trí ghế của đồ vật    | `seat_flip` | Hai bản ghi khác nhau giữa `rear_right` và `rear_left`. Giữ `rear_right` theo quy ước gọi ghế theo hướng xe. | Giữ nguyên |
| D01.png     | Điểm khóe miệng phải     | `flag`      | Hai bản khác cờ `outside`. Giữ điểm khóe miệng phải là điểm định vị được                                     | Giữ nguyên |
| D04.png     | Điểm khóe ngoài mắt trái | `flag`      | Giữ `outside=1` vì không định vị được điểm này.                                                              | Giữ nguyên |

## 2. Lỗi từng lặp lại

## 3. Ghi chú về disagreement_log

Nếu vẫn định vị được điểm thì dùng `occluded`. Nếu không đủ căn cứ để định vị thì dùng `outside`.
