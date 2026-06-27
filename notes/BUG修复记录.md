---
tags:
  - 故障排除
  - 修复
  - 修复bug
---
## git
- 出现网络问题时可以尝试取消 git 代理
```
git config --global --unset http.proxy && git config --global --unset https.proxy
``` 