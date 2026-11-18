# 鸣潮主线剧情

《鸣潮》主线的 TXT 阅读稿和 JSON 合集。从《万象新声》到《予以明日的花束》，共 **44 节、80 个主线任务**。TXT 按章、节和任务拆分，JSON 按相同顺序汇总为一个 UTF-8 文件。

[打开分块索引](主线分块索引.md) · [下载分块 ZIP](https://github.com/WinterMoonlight/wuwa-main-story/releases/download/snapshot-3.8.11/wuwa-main-story-3.8.11.zip) · [下载单文件 TXT](https://github.com/WinterMoonlight/wuwa-main-story/releases/download/snapshot-3.8.11/wuwa-main-story-full-3.8.11.txt) · [下载主线 JSON](https://github.com/WinterMoonlight/wuwa-main-story/releases/download/snapshot-3.8.11/wuwa-main-story-full-3.8.11.json) · [解析器源码](https://github.com/WinterMoonlight/wuwa-story-parser)

> [!NOTE]
> 文本来自 ConfigDB 3.8.11 快照，包含剧透。阅读稿保留原有缺口、可选交谈和顺序待核提示。

## 阅读方式

在 [TXT版](TXT版/) 按章、节浏览，或从[分块索引](主线分块索引.md)直接点开任务。下载分块 ZIP 后，可用压缩包内附的索引阅读。目录中的节号表示阅读位置，文件头同时保留游戏原幕名。

```text
TXT版/
  00_序幕/
  01_第一章/
  02_第二章/
  03_第三章/
  04_第四章/
JSON版/
  wuwa-main-story-full-3.8.11.json
主线分块索引.md
```

每份 TXT 开头标注章、节、全局阅读序号和任务 ID。连读顺序依据任务前置条件、已核对的回顾和章节树整理。顺序依据不足的位置在索引和相关任务开头注明。

合集位于 [JSON版](JSON版/)，按 `chapters[].sections[].tasks[].events[]` 组织。`quest_id` 是任务 ID，任务的 `sequence` 是全局阅读序号，事件的 `sequence` 是任务内序号。`kind` 区分对白、选项、字幕和提示等条目，`speaker` 和 `text` 分别保存说话人和正文。没有标注说话人的条目使用 `null`。

## 收录范围

本批整理简体中文主线，采用一条可阅读路线。追月节活动与乘霄山总回顾可通过原解析器的独立入口查看。数据库和客户端文件仍由使用者在本地管理。

这是一份非官方整理，游戏文本的权利归原权利人。解析器仓库的 MIT 许可证适用于其原创源码和文档。发现索引错位或文字问题，可以在 [Issues](https://github.com/WinterMoonlight/wuwa-main-story/issues) 提供任务 ID 和所在文件。
