# yt2obsidian

## 作用

`yt2obsidian` 会把一个 YouTube 链接整理成一篇 Obsidian 笔记：

- 下载英文字幕
- 清洗 VTT 里的时间轴和重复片段
- 生成 Markdown 笔记
- 自动更新对应目录下的 `Index.md`

默认行为是不改写字幕内容，只做结构整理，方便在 Obsidian 和 GitHub 里阅读。

## 前提

- 已安装 `yt-dlp`
- 已安装并启用 `obsidian` CLI
- 本机 Chrome 可以读取登录态
- 默认使用的 Chrome profile 是 `Profile 3`
- 默认固定写入 `language` vault（`/home/acheao/Work/language`）

脚本不再依赖当前激活的 Obsidian vault；即使你当前切在别的库，生成内容也会写进 `language`。

如果某个视频触发 YouTube 的 bot 检查，命令会优先尝试读取 Chrome cookie。这个策略已经在当前机器上验证过。

## 用法

```bash
yt2obsidian "<youtube-url>"
```

常用参数：

- `--folder "English/material/other"`：指定笔记落到 `language` vault 内的哪个目录
- `--profile "Default"`：改用别的 Chrome profile 读取 cookie
- `--title "..."`：手动指定笔记标题，覆盖 YouTube 返回的不稳定标题
- `--no-cookies`：完全不读浏览器 cookie
- `--open`：创建完成后直接在 Obsidian 打开笔记

## 示例

```bash
yt2obsidian "https://www.youtube.com/watch?v=D0UBAOensKo"
```

```bash
yt2obsidian "https://www.youtube.com/watch?v=D0UBAOensKo" --open
```

```bash
yt2obsidian "https://www.youtube.com/watch?v=D0UBAOensKo" --folder "English/material/other"
```

```bash
yt2obsidian "https://www.youtube.com/watch?v=oj5Tc45R06o" --title "Are YOU Making These 5 EASILY FIXABLE Common Mistakes in English?"
```

## 输出规则

- 默认会根据 YouTube channel 名称，把笔记放进 `English/material/<Channel>/`
- 如果对应文件夹已经存在，会直接复用那个文件夹
- 如果文件夹不存在，会自动创建文件夹和 `Index.md`
- 标题会优先尝试读取浏览器渲染后的页面标题，失败时再回退到元数据接口
- 新生成的文件名默认会带上视频 ID，格式类似 `Title [video-id].md`
- 新笔记会自动加入该目录的 `## Notes` 索引

生成出来的笔记结构是：

```md
# 视频标题

## Source
- URL: ...
- Channel: ...
- Subtitle source: ...

## Transcript
...
```

## 限制

- 目前只处理 YouTube 已有的英文字幕或英文自动字幕
- 还没有接入音频转写兜底，所以没有字幕的视频会失败
- `ffmpeg` 不参与当前流程
- 字幕如果本身没有标点，命令不会强行改写成润色稿

## 排错

如果下载失败，优先检查下面几项：

- Chrome 的目标 profile 是否是你当前登录 YouTube 的那个
- 视频是否有英文字幕或英文自动字幕
- `yt-dlp` 是否还能正常访问 YouTube

最常用的排错方式是换一个 profile 再试：

```bash
yt2obsidian "<youtube-url>" --profile "Default"
```
