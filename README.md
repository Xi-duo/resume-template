# 前端简历模板 · Frontend Resume Template

一份单文件 HTML 简历模板，无依赖、可直接打印为 A4 PDF。

**[在线预览 →](https://xi-duo.github.io/resume-template)**

---

## 特点

- **零依赖** — 纯 HTML + CSS，浏览器直接打开，不需要 Node / 构建工具
- **A4 打印优化** — `Cmd/Ctrl + P` 导出 PDF，排版不变形
- **Design Tokens** — 所有颜色/字体用 CSS 变量定义，一处修改全局生效
- **技术词高亮** — `<em>` 标签自动渲染为蓝色 badge，突出技术关键词
- **响应式** — 移动端可正常浏览
- **中文排版优化** — 字体栈覆盖 PingFang SC / 微软雅黑 / 系统默认

---

## 快速开始

1. 下载 `index.html`
2. 用任意编辑器打开，按注释填写个人信息
3. 浏览器打开预览
4. `Cmd/Ctrl + P` → 存为 PDF

---

## 自定义主题色

找到文件顶部的 `:root`，修改 `--color-accent` 即可：

```css
:root {
  --color-accent: #2563eb;  /* 默认蓝色 */

  /* 其他选择 */
  /* --color-accent: #7c3aed;  紫色 */
  /* --color-accent: #059669;  绿色 */
  /* --color-accent: #dc2626;  红色 */
  /* --color-accent: #d97706;  橙色 */
}
```

---

## 写作技巧

### bullet 格式
每条经历用 STAR 格式（情境 → 行动 → 结果），尽量有量化数字：

```
做了什么（用 <strong> 标记关键词），
通过 <em>技术方案</em> 解决了什么问题，
结果：<strong>性能提升 XX%</strong> / 延迟从 Xs 降至 Xms。
```

### 技术词高亮
`<em>` 标签在这份模板里不是斜体，而是蓝色 badge：

```html
通过 <em>WebSocket 预热</em> 将延迟从 <strong>3s 降至 750ms</strong>
```

### 核心技能标注
技能区的 `accent` class 表示核心/熟练技能，加蓝色背景：

```html
<span class="tag accent">React</span>   <!-- 核心技能 -->
<span class="tag">Vue</span>             <!-- 了解/使用过 -->
```

---

## 文件结构

```
index.html   ← 全部内容在这一个文件里，CSS 内嵌在 <style> 标签中
```

---

## License

MIT — 随意使用和修改，不需要署名。
