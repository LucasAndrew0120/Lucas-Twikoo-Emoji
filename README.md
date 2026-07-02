# Lucas-Twikoo-Emoji

[Twikoo](https://github.com/imaegoo/twikoo) 表情包合集，包含百度贴吧经典表情与精华表情，通过 jsDelivr CDN 加速。

## 表情包列表

- **Tieba-Classic** — 贴吧经典表情 (`tieba_classic/`)
- **Tieba-Refined** — 贴吧精华表情 (`tieba_refined/`)
- **小黄鸡** — 小黄鸡贴纸 (`xhj_stickers/`)

## 使用方法

将对应目录下的 JSON 文件内容粘贴到 Twikoo 后台「自定义表情」配置中即可，格式为：

```json
{
  "表情包名称": {
    "type": "image",
    "container": [
      {
        "text": "Tieba-Classic-1",
        "icon": "<img src='https://cdn.jsdelivr.net/gh/LucasAndrew0120/Lucas-Twikoo-Emoji@main/tieba_classic/image_emoticon.png'>"
      }
    ]
  }
}
```

## 爬取工具

`scrape_tieba_emoji.py` 用于从百度贴吧 CDN 批量下载表情：

```bash
python scrape_tieba_emoji.py
```

会自动下载图片并按照 Twikoo JSON 格式生成配置文件。
