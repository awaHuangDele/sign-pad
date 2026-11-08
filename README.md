# 签名板 · Sign Pad

一个单文件的网页手写签名板。打开就能写，写完导出透明 PNG，直接插进 Word、PDF 或线上表单。

> A single-file browser-based signature pad. Draw with mouse, touch or stylus, export a transparent PNG. No build, no dependencies, no network.

## 特点

- **单文件** — 只有 `index.html`，双击即用，也可以直接扔到任意静态托管
- **不联网** — 没有任何网络请求：无 CDN、无字体外链、无埋点。断网可用，笔迹不出本机
- **高清导出** — 2 倍超采样，透明 PNG 实际尺寸 2400 × 840
- **笔迹连续** — 中点二次贝塞尔，段与段首尾相接不留缝；合并事件全量取点，快速划动也不断线
- **可调笔迹** — 黑色 / 蓝黑 / 蓝，线宽 1.5–8 px
- **可撤销** — 最多回退 6 步，支持整张清空
- **可选日期** — 勾选后在签名右下方自动附上日期
- **两种底色** — 透明 PNG（叠在文档上不遮字）/ 白底 PNG（部分系统对透明底兼容差）

## 用法

打开 `index.html`，或访问 GitHub Pages 在线版。

1. 在框里手写签名
2. 按需调整颜色和粗细
3. 导出 PNG，插入 Word（设为「浮于文字上方」）或 PDF（WPS / Acrobat 的签名功能）

## 拿它签承诺书之前

- 签名用**黑色**签字笔的笔迹效果最自然，日期也建议手写
- 承诺书如果写着「已阅读并抄写全文」，必须**真笔手写**，图片签名不成立
- 需要按手印的（社区、学校常见），打印 → 签字 → 按印泥 → 拍照
- 线上表单上传白底 PNG 兼容性更好，有些系统会把透明底渲染成黑块

## 浏览器支持

Chrome / Edge / Firefox / Safari 近两年版本。依赖 Pointer Events 与 Canvas，无需 WebGL。

## License

[MIT](LICENSE)
