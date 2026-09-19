---
layout: post
title: "Mẹo nhỏ: kiểm tra pin laptop có bị chai không mà không cần cài phần mềm"
date: 2026-08-20 20:00:00 +0700
excerpt: "Đào lại thói quen cũ thời còn viết blog thủ thuật — lần này là một lệnh Windows có sẵn, không cần tải gì thêm."
tags: ["mẹo IT","Windows"]
published: true
---

Đào lại thói quen cũ thời còn viết blog thủ thuật máy tính — lần này là một mẹo mình vẫn hay dùng khi còn làm kĩ thuật viên: kiểm tra pin laptop có bị chai không mà không cần cài thêm phần mềm nào cả, Windows đã có sẵn công cụ này.

## Cách làm

1. Mở **Command Prompt** (gõ `cmd` ở ô tìm kiếm)
2. Gõ lệnh sau rồi Enter:

```bat
powercfg /batteryreport
```

3. Windows sẽ tạo ra một file HTML báo cáo, thường nằm ở:

```bat
C:\Users\<tên-người-dùng>\battery-report.html
```

4. Mở file đó bằng trình duyệt, kéo xuống mục **Design Capacity** (dung lượng pin lúc xuất xưởng) và **Full Charge Capacity** (dung lượng sạc đầy thực tế hiện tại).

## Cách đọc kết quả

- Hai số càng gần nhau → pin còn khoẻ
- Full Charge Capacity càng thấp hơn Design Capacity nhiều → pin càng chai
- Chênh lệch quá lớn (trên 40-50%) thì nên cân nhắc thay pin, vì lúc đó thời lượng dùng thực tế đã giảm khá nhiều so với quảng cáo ban đầu

Mẹo này mình dùng cho khách khá nhiều hồi còn ở Máy tính Quảng Ninh — nhanh, không cần cài gì, không lo phần mềm lạ.
