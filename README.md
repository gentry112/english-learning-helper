# 六级词汇翻译助手

面向 CET-6 备考学生的移动端网页查词工具。输入英文词汇/短语/句子，自动完成拼写纠错、释义拆解、六级频率评估、学习记录和考试扩展。

## 功能

- **拼写检查与纠错** — 自动检测拼写错误，给出纠正建议
- **完整释义** — 短语/句子整体中文释义 + 逐词拆解（原形、词性、释义、派生词）
- **六级频率标注** — 高频🔴 / 中频🟡 / 低频🟢，含近5年真题出现情况说明
- **学习记录** — 自动记录查询历史，重复查询提示累计次数
- **六级扩展** — 常考搭配、真题例句、近义词辨析、写作高级替换表达
- **学习项目管理** — 多文件夹管理（按真题年份/篇目分类），每文件夹独立记录 + 重点词汇汇总（综合权重排序）

## 使用方法

### 方式一：直接打开

1. 下载 `index.html`
2. 用浏览器直接打开
3. 点击右上角 ⚙️ 设置你的 DeepSeek API Key
4. 开始查词

### 方式二：静态托管

将 `index.html` 部署到 GitHub Pages / Vercel / Netlify 等静态托管平台。

## 技术栈

- Vue 3（CDN 引入）
- Tailwind CSS（CDN Play）
- DeepSeek API（前端直调）
- localStorage 数据持久化
- 单文件 HTML，无构建工具，无后端

## 数据存储

所有数据存储在浏览器 localStorage：
- `cet6-api-key`：DeepSeek API Key
- `cet6-folders`：文件夹与词汇查询历史

> ⚠️ 清除浏览器数据会导致记录丢失。

## API Key

需要自行申请 DeepSeek API Key：https://platform.deepseek.com/

API Key 在设置弹窗中输入，保存到 localStorage，严禁硬编码在代码中。

## 项目文档

- [需求收集](PRDS/requirements.md)
- [产品需求文档](PRDS/PRD.md)
- [UI 设计文档](PRDS/UI.md)
- [技术架构文档](PRDS/tech.md)
