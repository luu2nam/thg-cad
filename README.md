# THG CAD — plugin AutoCAD 2025 / 2026 / 2027

Sản phẩm của **Phòng KCM - Công ty Than Hòn Gai - TKV**: bộ công cụ AutoCAD cho bản vẽ mỏ.

Kho này **chỉ chứa bộ cài** (mục [Releases](../../releases)). Mã nguồn không công khai.

## Tính năng

| Lĩnh vực | Có gì |
|---|---|
| **Lộ thiên** | Nhập điểm máy đo (TXT/CSV, tự đổi X/Y VN-2000), kiểm tra số liệu điểm cos, bề mặt TIN theo kỳ, đồng mức, mặt 3D, xem 3D so sánh các kỳ; hệ tuyến và mặt cắt nhiều bề mặt (tô đào / đắp, mức tầng, dải số liệu); kế hoạch trên mặt cắt (vẽ, sửa đỉnh, lên bình đồ, xuất toạ độ); khối lượng giữa 2 bề mặt theo mức, tách than, xuất Excel; cung độ vận chuyển bình quân; thiết kế tầng, taluy, dốc đường |
| **In ấn** | Bôi đen là nhận khung, in PDF hàng loạt đúng khung, ghép 1 PDF có mục lục, sẵn sàng ký số; hồ sơ in dùng chung cả phòng; in máy in giấy / plotter |
| **Tiện ích** | Chuẩn hóa layer bản vẽ cũ về chuẩn layer THG, danh mục layer chuẩn dùng chung |
| Hầm lò, Thông gió | Đang phát triển |

Trong AutoCAD: tab **THG CAD** trên Ribbon → **Hướng dẫn** — hướng dẫn từng bước, có nút "▶ Làm ngay" chạy thử trên bản vẽ.

## Cài đặt
1. Vào [Releases](../../releases/latest), tải `THG-Setup-x.y.z.exe`.
2. **Lưu bản vẽ và đóng AutoCAD.**
3. Bấm đúp bộ cài, chọn **Cài cho mọi người trên máy** (khuyên dùng, cần quyền quản trị) — AutoCAD không hỏi "Load / Do Not Load" mỗi lần mở.
   Không có quyền quản trị: chọn **Chỉ cài cho tôi**, khi AutoCAD hỏi thì bấm "Always Load".
4. Mở AutoCAD → tab **THG CAD** → **Hướng dẫn** → đọc bài **"Bắt đầu: làm quen THG CAD"**.

## Dùng thử và kích hoạt
- Cài xong được **dùng thử 7 ngày** (lần đầu mở AutoCAD có mạng Internet), đủ mọi tính năng.
- Sau đó nhập **mã kích hoạt** dạng `THG-XXXX-XXXX-XXXX` (xin Phòng KCM): tab **THG CAD → Kích hoạt**.
- Đã kích hoạt thì dùng được không cần mạng tối đa 30 ngày; có mạng plugin tự gia hạn.
- Đổi máy: cửa sổ Kích hoạt → **Hủy kích hoạt máy này**, rồi kích hoạt máy mới bằng cùng mã.

## Cập nhật
- Có bản mới thì lúc mở AutoCAD plugin **tự nhắc**: cửa sổ "Có bản mới" và biểu tượng THG ở thanh trạng thái góc dưới phải.
  Bấm **Tải và cài đặt** → đồng ý đóng AutoCAD → mở lại. Có thể chọn **Nhắc lại sau** hoặc **Bỏ qua bản này**.
- Kiểm tra bất cứ lúc nào: tab **THG CAD → Kiểm tra cập nhật**. Plugin không tự tải, không tự cài.
- Sau khi cập nhật, cửa sổ **"Có gì mới"** tóm tắt thay đổi (xem lại: lệnh `THG_COGIMOI`).
- Máy không có Internet: tải bộ cài mới ở máy khác, cài đè như lần đầu (không cần gỡ). Cấu hình riêng không bị mất.

## Gỡ cài đặt
Windows **Settings → Apps → "THG CAD"**.

## Báo lỗi
Tab **THG CAD → Thông tin**: lấy đường dẫn file nhật ký lỗi `thg.log`, gửi kèm ảnh chụp màn hình và mô tả cho Phòng KCM.

## Kiểm tra file tải về (tùy chọn)
Mỗi bản phát hành kèm file `.sha256`. Kiểm tra trong PowerShell:
```
Get-FileHash .\THG-Setup-x.y.z.exe -Algorithm SHA256
```
