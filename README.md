# Happening Now

判断一件事是否每分每秒都在发生 —— 一个交互式 Web 应用。

输入任意事件（如"有人正在喝可口可乐"），应用会通过 LLM 分析该事件的全球发生频率，并在 3D 地球上实时展示。

## 功能

- **3D 地球可视化** -- 基于 Canvas 的交互式地球，包含大陆、海洋、星空、大气层和云层
- **LLM 智能分析** -- 接入 OpenAI 兼容 API，分析事件的全球发生频率
- **实时计数器** -- 从分析开始自动累计事件发生次数
- **频率对比图表** -- 柱状图直观对比不同事件的发生频率
- **中英文切换** -- 支持中文和英文界面
- **深色/浅色主题** -- 一键切换，自动记忆偏好
- **预设事件** -- 内置 5 个热门事件快速体验

## 快速开始

直接在浏览器中打开 `index.html` 即可使用。

无需安装依赖，无需构建步骤。

## 配置 API

1. 点击页面底部的 **⚙ API 设置**
2. 填入：
   - **API 地址** -- OpenAI 兼容的 Chat Completions 端点（如 `https://api.openai.com/v1/chat/completions`）
   - **API Key** -- 你的 API 密钥
   - **模型名称** -- 如 `gpt-4o`
3. 点击 **保存设置**

API 配置保存在浏览器 localStorage 中，不会上传到任何服务器。

## 项目结构

```
index.html    -- 页面结构
style.css     -- 样式与主题变量
app.js        -- 应用逻辑（主题、i18n、地球渲染、LLM 调用）
```

## 技术栈

- 原生 HTML / CSS / JavaScript
- Canvas 2D 地球渲染
- OpenAI 兼容 API（Chat Completions）
- CSS 变量实现主题切换
- 无外部依赖

## License

MIT
