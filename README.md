<p align="center">
  <img src="assets/icon.png" width="96" alt="TransLift 图标" />
</p>

<h1 align="center">Zotero TransLift 插件</h1>

<p align="center">
  Zotero 内的 AI 翻译与阅读插件：全文翻译、划词翻译、双语对照、AI 助手、AI 大纲。
</p>

<p align="center">
  <a href="https://github.com/zwjjiaozhu/Zotero-TransLift/releases/latest"><img src="https://img.shields.io/github/v/release/zwjjiaozhu/Zotero-TransLift?label=release&style=flat-square" alt="latest release" /></a>
  <a href="https://www.zotero.org"><img src="https://img.shields.io/badge/Zotero-7%20%E2%80%93%2011-CC2936?style=flat-square&logo=zotero&logoColor=white" alt="Zotero 7-11" /></a>
  <a href="https://github.com/zwjjiaozhu/Zotero-TransLift/releases"><img src="https://img.shields.io/github/downloads/zwjjiaozhu/Zotero-TransLift/total?label=downloads&style=flat-square" alt="downloads" /></a>
</p>

<p align="center">
  <a href="https://www.jztranslate.com">官网</a> ·
  <a href="https://docs.jztranslate.com">使用文档</a> ·
  <a href="https://github.com/zwjjiaozhu/Zotero-TransLift/releases">下载插件</a> ·
  <a href="https://github.com/zwjjiaozhu/Zotero-TransLift/issues">反馈问题</a>
</p>

---

## 这是什么

在 Zotero 里读文献时的翻译层：打开 PDF 就能整篇翻译，选中一句话就能划词翻译，也可以把原文和译文上下/左右对照着读；侧边栏和划词悬浮球里还接了 AI 助手，可以直接对选中的段落做解释、翻译、总结。

## 功能

| 功能 | 说明 |
| --- | --- |
| 全文翻译 | PDF、Docx 等整篇文档翻译，带进度显示与失败重试，可导出译文 |
| 划词翻译 | 选中文字松手即译，可切换引擎、多选对照；支持弹窗与侧边栏两种呈现，也可用悬浮球触发 |
| 双语对照阅读 | 上下对照 / 左右对照 / 仅译文三种模式，段落与句子级一一高亮，背景色跟随 Zotero 主题 |
| AI 助手 | 侧边栏对话：解释、翻译、总结、自定义提示词；支持 ChatGPT、Gemini、豆包、元宝等网页端接入 |
| AI 大纲 | 为论文生成结构大纲，点击可跳转到对应位置 |
| 朗读 | 逐句朗读与原文/译文跟随高亮，可切换 TTS 引擎 |
| 多引擎 | 内置 DeepL、百度、必应、Google、彩云、火山、腾讯交互翻译、Papago、Yandex、搜狗、知网、饺子等翻译通道 |

## 安装

1. 到 [Releases](https://github.com/zwjjiaozhu/Zotero-TransLift/releases/latest) 下载 `trans-lift.xpi`。
2. Zotero 菜单栏 → `工具` → `附加组件和插件`。
3. 点右上角齿轮 → `从文件安装附加组件...`，选择刚下载的 `.xpi`。
4. 重启 Zotero，首次使用时登录饺子账号。

插件内置自动更新：Zotero 会在有新版本时提示升级，无需手动重装。

## 版本要求

- Zotero **7 – 11**。
- 双语对照阅读依赖 Zotero 10 及以上的阅读模式能力；在 Zotero 7 – 9 下使用该项会提示不支持，其余功能不受影响。

## 账号与费用

插件本身免费提供下载和安装，翻译与 AI 能力的用量按饺子账号的免费额度 / 会员计费，具体见 [官网](https://www.jztranslate.com)。部分翻译通道也支持在设置里填写你自己的接口参数（如百度 `appid` + `key`、DeepL 等），此时不消耗饺子账号额度。

## 数据说明

翻译、文档解析和 AI 对话请求，会把对应的文本内容发送到你选择的引擎服务端或 `jztranslate.com` 服务端。除完成这些功能所必需的数据外，插件不额外上传文库内容。

## 常见问题

- **装了没反应**：确认 Zotero 已重启，并在 `工具 → 附加组件和插件` 中看到 TransLift 处于启用状态。
- **双语对照打不开**：检查 Zotero 版本是否 ≥ 10，以及当前是否处于阅读模式。
- **翻译失败**：多数是接口限流或额度用尽，条目右侧会出现重试按钮；也可以切换到其他引擎。

更细的用法见 [使用文档](https://docs.jztranslate.com)。

## 本仓库说明

这是 TransLift 的**发行仓库**：用于托管安装包、版本说明和问题反馈，插件源码不在本仓库公开。

- [dist/trans-lift-2.9.3.xpi](https://github.com/zwjjiaozhu/Zotero-TransLift/raw/main/dist/trans-lift-2.9.3.xpi) — 安装包直链，内容与 Releases 一致。
- [CHANGELOG.md](CHANGELOG.md) — 版本更新说明。

## 许可

本仓库内文档按 [LICENSE](LICENSE) 授权；插件安装包（`.xpi`）为闭源分发型软件，最终用户条款见 [官网](https://www.jztranslate.com)。
