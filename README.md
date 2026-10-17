# THG CAD — plugin AutoCAD 2025 / 2026 / 2027

Sản phẩm của **Phòng KCM - THG**: in ấn PDF, lộ thiên (bề mặt 3D, mặt cắt, khối lượng, cung độ, thiết kế tầng), chuẩn hóa layer.

Kho này **chỉ chứa bộ cài** (mục [Releases](../../releases)). Mã nguồn không công khai.

## Cài đặt
1. Vào [Releases](../../releases/latest), tải `THG-Setup-x.y.z.exe`.
2. **Lưu bản vẽ và đóng AutoCAD.**
3. Bấm đúp bộ cài, chọn **Cài cho mọi người trên máy** (khuyên dùng, cần quyền quản trị) — AutoCAD không hỏi "Load / Do Not Load" mỗi lần mở.
   Không có quyền quản trị: chọn **Chỉ cài cho tôi**, khi AutoCAD hỏi thì bấm "Always Load".
4. Mở AutoCAD → tab **THG CAD** trên Ribbon → **Hướng dẫn**.

## Cập nhật
Trong AutoCAD: tab **THG CAD** → **Kiểm tra cập nhật**. Plugin không tự cập nhật ngầm.

## Gỡ cài đặt
Windows **Settings → Apps → "THG CAD"**.

## Kiểm tra file tải về (tùy chọn)
Mỗi bản phát hành kèm file `.sha256`. Kiểm tra trong PowerShell:
```
Get-FileHash .\THG-Setup-x.y.z.exe -Algorithm SHA256
```
