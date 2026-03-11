## 描述

希望在聊天窗口中，当用户发送图片URL（如 .jpg, .png, .gif 等）时，能够自动渲染成图片显示，而不是显示纯文本链接。

## 期望行为

用户发送 `https://example.com/image.png` 时，聊天窗口应该直接显示这张图片。

## 技术建议

在消息渲染时，检测文本内容是否为图片URL（正则匹配 jpg/jpeg/png/gif/webp/svg 等格式），如果是则转换为 `<img>` 标签显示。

或者可以利用现有的 `X0` 函数处理图片的逻辑。

## 其他

感谢 OpenClaw！用起来很棒！

---

**可直接复制到 GitHub Issue:**
https://github.com/openclaw/openclaw/issues/new
