# 🌏 生物钟属地计算器 (Bio-Clock Citizenship)

> **💡 Note:** 本项目主体逻辑由人类编写，前端实现使用了 **Gemini 3** 辅助。

---

**生物钟属地计算器**是一个基于 React 的 Web 应用。它根据你的“起床时间”和“当前所在地”，通过计算时差，寻找世界上哪个城市的作息节奏最符合你的生物钟，并生成分享卡片。

## ✨ 主要功能

* **⏱️ 跨时区匹配**：根据 UTC 偏移量，精确计算你的生物钟属于哪个城市（支持全球 10+ 个代表性城市）
* **🗣️ 双语支持**：完整的中/英文界面与文案切换
* **💬 趣味点评**：根据匹配结果提供带有当地文化特色的点评
* **🖼️ 生成分享卡**：一键生成结果图片


## 🛠️ 技术栈 (Tech Stack)

* **Core**: React 18 + ReactDOM (UMD CDN 版本)
* **Compiler**: Babel Standalone (浏览器端实时编译 JSX)
* **Styling**: Tailwind CSS (CDN 版本)
* **Utils**:
* `html2canvas`: 用于 DOM 截图生成分享海报。
* `qrcode.js`: 生成当前页面的二维码。
* `Intl.DateTimeFormat`: 原生 JavaScript API 处理时区逻辑。

## 🤝 自定义

想添加更多城市？只需在 `script` 标签内的 `citiesData` 数组中添加对象即可：

```javascript
{ 
    id: "Paris", 
    timezone: "Europe/Paris", 
    code: "fr", 
    region: { zh: "法国", en: "France" } 
}

```

并记得在 `translations.regionComments` 中添加对应的趣味文案！

## 📄 开源协议

MIT License. 随意修改，祝你玩得开心！

---
