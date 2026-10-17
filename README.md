# THG — plugin AutoCAD 2027

Plugin AutoCAD của **phòng KCM, Công ty CP Than Hòn Gai - TKV**: in ấn PDF, lộ thiên (bề mặt 3D, mặt cắt, khối lượng,
cung độ, thiết kế tầng), chuẩn hóa layer.

Kho này **chỉ chứa bộ cài** (mục [Releases](../../releases)). Mã nguồn không công khai.

## Cài đặt
1. Vào [Releases](../../releases/latest), tải `THG-Setup-x.y.z.exe`.
2. **Lưu bản vẽ và đóng AutoCAD.**
3. Bấm đúp bộ cài:
   - **Cài cho mọi người trên máy** (cần quyền quản trị) — AutoCAD không hỏi "Load / Do Not Load" mỗi lần mở. Khuyên dùng.
   - **Chỉ cài cho tôi** — không cần quyền quản trị; lần mở AutoCAD đầu tiên bấm "Always Load".
4. Mở AutoCAD 2027 → tab **THG** trên Ribbon → **Hướng dẫn**.

## Cập nhật
Trong AutoCAD: tab **THG** → **Kiểm tra cập nhật**. Plugin không tự cập nhật ngầm.

## Gỡ cài đặt
Windows **Settings → Apps → "THG - Than Hòn Gai"**.

## Kiểm tra file tải về (tùy chọn)
Mỗi bản phát hành kèm file `.sha256`. Kiểm tra trong PowerShell:
```
Get-FileHash .\THG-Setup-x.y.z.exe -Algorithm SHA256
```
