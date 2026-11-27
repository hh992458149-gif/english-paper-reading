# 英文文献对照精读

给用中文读英文论文的人。把 PDF 或当前读到的一段交给 Codex，选中一个词、一个公式或一张图，就从那里讲起。下次换个对话，也可以从上次停下的那句继续。

*An Agent Skill for reading English research papers in Chinese, with bilingual explanations and sentence-level reading notes.*

## 先试读一分钟

胡克在显微镜下观察一片很薄的软木，把切面上的孔隙比作蜂巢。读者问，原文里的 *regular* 怎么翻译？

在这一句里，它说的是孔隙的形状是否**规整**。蜂巢的比喻让人想到许多相邻的小空腔，作者紧接着又指出了两者的差别。这样读，就能把显微镜下看见的结构和打比方时借用的形状分开。

下载试读页，用浏览器打开即可切换中英对照、调整字号、保存段落书签。已经安装技能的读者可以直接双击安装目录里的 `assets/reader.html`。想追问某个词时，选中并复制它所在的英文片段，和问题一起粘贴到 Codex。[下载离线试读页](https://github.com/hh992458149-gif/english-paper-reading/raw/refs/heads/main/skills/english-paper-reading/assets/reader.html)

节选取自 Robert Hooke 的 *Micrographia*，第 XVIII 则，1667 年印本书内第 113 页。[原书扫描](https://www.microscopemuseum.eu/books/Robert_Hooke_1667_Micrographia_or_Some_physiological_descriptions_of_minute_bodies_made_by_magnifying_glasses.pdf)

## 安装到 Codex

在 Codex 里发送这一句。

```text
用 $skill-installer 从 https://github.com/hh992458149-gif/english-paper-reading/tree/main/skills/english-paper-reading 安装这个技能。
```

也可以下载仓库，把 `skills/english-paper-reading` 整个文件夹复制到用户主目录下的 `.agents/skills/`。打开一个新对话，输入 `$english-paper-reading` 即可点名使用。[Codex 技能安装说明](https://developers.openai.com/codex/skills/)

## 三种用法

| 读到哪一步 | 可以直接对 Codex 说 |
| --- | --- |
| 卡在一句或一张图上 | “用 $english-paper-reading 讲我选中的这句。先翻译，再解释作者为什么用这个词，以及图 2 的哪组数据支持它。” |
| 想准备整篇材料 | “把这个 PDF 做成离线双语 HTML 和可批注的 Word，保留原图、表格和原 PDF 页码。我还在读摘要。” |
| 今天先读到这里 | “保存这篇的精读位置，记下下一句英文。” 下次在同一个项目里说“继续上次那篇”。 |

全文对照稿与实际精读进度分别记录。生成完整译稿后，仍从你真正读过的位置接续。篇末用三个问题收束阅读：论文发现了什么、哪些做法有新意？作者如何做实验，关键对照和参数是什么？哪些方法或结论值得放进自己的课题验证？

只读一段时，贴出文字即可。制作全篇需要在能读取原 PDF、写入本地文件并生成相应文档的环境中使用。离线 HTML 的书签存在当前浏览器，跨对话续读使用项目中的阅读记录。

## 反馈

欢迎留下一次具体体验，例如某张双栏表格哪里读乱了，或换个对话后是否回到了正确的那一句。公开论文给出链接和页码即可，未公开稿件可用自写短句重现。[提交阅读反馈](https://github.com/hh992458149-gif/english-paper-reading/issues/new?template=reading-feedback.yml)

当前版本公开试用，暂未附开源许可证。
