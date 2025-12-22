---
share: true
created: 2023-05-26T14:51
updated: 2025-12-22T17:32
title: Quản lý clipboard bằng CopyQ
---
## Copy tin nhắn từ Discord
```js
copyq:
var raw = str(clipboard())
var processed = raw.replace(new RegExp(" — .* at .*\n", "g"), ": ")
copy(processed)
paste()
```
