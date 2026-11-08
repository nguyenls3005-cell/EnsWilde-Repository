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
