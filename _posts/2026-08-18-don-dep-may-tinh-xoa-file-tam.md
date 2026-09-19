---
layout: post
title: "Dọn máy tính ì ạch: file tạm trốn ở đâu và xoá thế nào cho sạch"
date: 2026-08-18 20:00:00 +0700
excerpt: "Một mẹo cũ mà vẫn hiệu quả — máy chậm nhiều khi chỉ vì rác file tạm chất đống, không phải lúc nào cũng do phần cứng yếu."
tags: ["mẹo IT","Windows"]
published: true
---

Máy chậm nhiều khi không phải do cấu hình yếu, mà đơn giản là rác file tạm (temp) chất đống qua thời gian. Mỗi lần cài phần mềm, Windows update, hay trình duyệt chạy, đều để lại ít nhiều file tạm — gom lại có khi tới vài GB.

## Xoá nhanh bằng hộp thoại Run

Nhấn `Windows + R`, gõ lần lượt các lệnh sau (mỗi lệnh xong thì xoá hết những gì hiện ra trong thư mục mở lên):

```bat
%temp%
```

```bat
temp
```

```bat
prefetch
```

## Lưu ý nhỏ

- Một vài file trong các thư mục này có thể đang được chương trình khác sử dụng — nếu Windows báo không xoá được thì cứ bỏ qua, không cần cố ép
- Nên làm định kỳ, khoảng 1-2 tháng một lần, thay vì đợi máy ì ạch hẳn mới dọn
- Cách này an toàn hơn nhiều so với mấy phần mềm "dọn rác" quảng cáo linh tinh mà mình từng thấy hồi xưa hay giới thiệu trên blog cũ (¬‿¬)
