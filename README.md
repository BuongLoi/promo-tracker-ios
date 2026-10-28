# 🏷️ Promo Tracker — iOS Native App (`Kiểm Tra Chương Trình Khuyến Mãi v1.0`)

> **Promo Tracker iOS Native Wrapper**  
> Ứng dụng tra cứu, lọc đa chiều, quét mã vạch sản phẩm và cập nhật file Excel khuyến mãi hàng ngày tại [https://buongloi.loc.cc](https://buongloi.loc.cc) — hỗ trợ **Dark Mode & Light Mode**.

---

## 📱 Thông Tin Ứng Dụng

| Hạng mục | Chi tiết |
|---|---|
| **Tên ứng dụng** | Promo Tracker |
| **Bundle Identifier** | `me.buongloi.promotracker` |
| **Phiên bản** | `1.0.0` (Build `1`) |
| **Yêu cầu hệ điều hành** | iOS 16.0 trở lên (Tương thích iPhone & iPad) |
| **Máy chủ Web App** | `https://buongloi.loc.cc` (VPS port `8098`) |
| **Hình thức đóng gói** | Unsigned IPA (Cài đặt qua ESign / TrollStore / AltStore / Sideloadly) |

---

## ✨ Tính Năng Nổi Bật Trên iOS

- **Tra cứu & Lọc đa chiều**: Lọc tức thì theo Sheet tháng (`08.2026`, `09.2026`, `10.2026`, `11.2026`...), Trạng thái thực tế, Hình thức KM, Cửa hàng/Site, Ngành hàng, MD Phụ trách, Người tạo.
- **Quét Camera Barcode & Hiện Mã Vạch POS**: Cấp quyền Camera trực tiếp trong `WKWebView` để quét mã vạch sản phẩm tại quầy, hoặc hiển thị mã vạch EAN-13/Code128 trên màn hình để máy POS quét kiểm tra giá.
- **Upload File Excel Hàng Ngày**: Chọn trực tiếp file `.xlsx` mới từ ứng dụng **Tệp (Files)** trên iPhone để cập nhật dữ liệu tức thì.
- **3D Touch / Haptic Touch Quick Actions**: Nhấn giữ biểu tượng ứng dụng để mở nhanh *Quét Mã Vạch SP*, *CTKM Sắp Hết Hạn*, hoặc *Cập Nhật File Excel*.

---

## 🚀 Cách Build File `.ipa` qua GitHub Actions

Dự án sử dụng **GitHub Actions** với runner `macos-14` + `Xcode 16` + `XcodeGen` để tự động biên dịch ra file `PromoTracker.ipa`.

### 1. Tự động khi Push code:
```bash
git add .
git commit -m "feat: update PromoTracker iOS v1.0"
git push origin main
```

### 2. Kích hoạt thủ công:
1. Truy cập mục **Actions**: [https://github.com/BuongLoi/promo-tracker-ios/actions](https://github.com/BuongLoi/promo-tracker-ios/actions)
2. Chọn workflow **`Build iOS (.ipa)`** ở cột trái.
3. Bấm **`Run workflow`** ➔ Chọn branch `main` ➔ Bấm **`Run workflow`**.
