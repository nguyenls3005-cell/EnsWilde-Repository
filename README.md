# EnsWilde Repository

> Kho JSON chứa danh sách **Passcode Theme** (`.passthm`) dùng cho **Theme Store** trong ứng dụng [EnsWilde](https://github.com/YangJiiii/EnsWilde) — công cụ tùy biến iOS không cần jailbreak.

[![Repo](https://img.shields.io/badge/repo-JSON-blue)](https://github.com/nguyenls3005-cell/EnsWilde-Repository)
[![Format](https://img.shields.io/badge/format-json-yellow)](./themes.json)
[![Themes](https://img.shields.io/badge/dynamic/json?url=https://raw.githubusercontent.com/nguyenls3005-cell/EnsWilde-Repository/main/themes.json&query=$.themes.length&label=themes&color=green)](./themes.json)

---

## 📖 Giới thiệu

**EnsWilde-Repository** là **nguồn cấp dữ liệu** cho tính năng **Theme Store** trong app EnsWilde. Khi người dùng mở Theme Store, app sẽ:

1. Tải file [`themes.json`](./themes.json) từ repo này.
2. Hiển thị danh sách theme kèm ảnh preview, mô tả và tác giả.
3. Khi người dùng chọn một theme, app tải file `.passthm` tương ứng và áp dụng lên thiết bị.

> ⚠️ **Đây là repo dữ liệu (JSON + assets), KHÔNG phải mã nguồn app.**
> Mã nguồn EnsWilde nằm tại: [LSNguyen/EnsWilde](https://github.com/nguyenls3005-cell/EnsWilde)

---

## 📁 Cấu trúc repository

| Đường dẫn | Mô tả |
|---|---|
| `themes.json` | File metadata chính chứa danh sách toàn bộ theme. |
| `assets/` | Ảnh preview (`*.png`) cho từng theme. |
| `package/` | File theme (`.passthm`) để app tải và cài đặt. |

---

## 📄 Định dạng `themes.json`

`themes.json` là một object JSON gồm **metadata của repository** và **mảng `themes`** — mỗi phần tử đại diện cho một theme.

### Cấu trúc tổng quát

```json
{
  "identifier": "identifer cua repo",
  "name": "ten repo cua ban",
  "icon": "icon cua repo",
  "themes": [
    {
      "id": x,
      "name": "ten cua theme",
      "description": "mo ta theme",
      "url": "noi tai theme ve",
      "preview": "hinh minh hoa",
      "authors": "ten tac gia"
    }
  ]
}