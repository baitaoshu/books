# 白桃书 · 公版书库

中国古典小说的**公版全文**，纯 Markdown 一章一个文件，可以直接在 GitHub 上读，也可以拿去自己搭站。

在线阅读 → **https://baitaoshu.com**

- **25 本**、**2184 篇**、约 **973 万字**
- 全部为公有领域作品（作者逝世逾 100 年），无版权问题
- 一本书一个目录：`README.md` 是目录页，`001.md`、`002.md`… 是各篇正文，篇末带上一章/下一章
- [`index.json`](index.json) 是机器可读的书目（slug / 作者 / 篇数 / 字数 / 简介 / 目录路径）

## 书目

| 书名 | 作者 | 类目 | 篇数 | 万字 |
|---|---|---|---|---|
| [红楼梦](books/hongloumeng/) | 曹雪芹 | 古典名著 | 120 | 86.5 |
| [西游记](books/xiyouji/) | 吴承恩 | 古典名著 | 100 | 73.0 |
| [三国演义](books/sanguoyanyi/) | 罗贯中 | 古典名著 | 120 | 59.5 |
| [儒林外史](books/rulinwaishi/) | 吴敬梓 | 古典名著 | 56 | 32.8 |
| [镜花缘](books/jinghuayuan/) | 李汝珍 | 古典名著 | 100 | 41.1 |
| [老残游记](books/laocanyouji/) | 刘鹗 | 古典名著 | 20 | 10.9 |
| [水浒传](books/shuihuzhuan/) | 施耐庵 | 古典名著 | 117 | 88.0 |
| [聊斋志异](books/liaozhaizhiyi/) | 蒲松龄 | 古典名著 | 496 | 48.5 |
| [封神演义](books/fengshenyanyi/) | 许仲琳（一说陆西星） | 古典名著 | 100 | 59.1 |
| [东周列国志](books/dongzhoulieguozhi/) | 冯梦龙（蔡元放修订） | 古典名著 | 110 | 67.7 |
| [隋唐演义](books/suitangyanyi/) | 褚人获 | 古典名著 | 100 | 62.3 |
| [说岳全传](books/shuoyuequanzhuan/) | 钱彩 | 古典名著 | 80 | 41.7 |
| [济公全传](books/jigongquanzhuan/) | 郭小亭 | 古典名著 | 240 | 70.0 |
| [官场现形记](books/guanchangxianxingji/) | 李宝嘉 | 古典名著 | 59 | 63.9 |
| [孽海花](books/niehaihua/) | 曾朴 | 古典名著 | 35 | 25.3 |
| [二十年目睹之怪现状](books/ershimuduzhiguai/) | 吴趼人 | 古典名著 | 108 | 54.5 |
| [海上花列传](books/haishanghualiezhuan/) | 韩邦庆 | 古典名著 | 66 | 31.5 |
| [厚黑学](books/houheixue/) | 李宗吾 | 国学 | 6 | 1.2 |
| [孙子兵法](books/sunzibingfa/) | 孙武 | 国学 | 13 | 0.8 |
| [三十六计](books/sanshiliuji/) | 檀道济（传） | 国学 | 7 | 0.7 |
| [鬼谷子](books/guiguzi/) | 鬼谷子（陶弘景注） | 国学 | 19 | 3.9 |
| [智囊](books/zhinang/) | 冯梦龙 | 国学 | 28 | 31.9 |
| [曾国藩家书](books/zengguofanjiashu/) | 曾国藩 | 国学 | 74 | 5.5 |
| [厚黑丛话](books/houheiconghua/) | 李宗吾 | 国学 | 8 | 10.4 |
| [厚黑余谈](books/houheiyutan/) | 李宗吾 | 国学 | 2 | 2.9 |

## 怎么用

**直接读**：点上面任意书名进目录页，再点回目进正文；每篇末尾有上一章 / 下一章，可以顺着读完。

**拉下来用**：

```bash
git clone https://github.com/baitaoshu/books.git
```

**程序化处理**：读 `index.json`，字段固定，不会变。

```json
{
  "slug": "hongloumeng",
  "title": "红楼梦",
  "author": "曹雪芹",
  "category": "古典名著",
  "chapters": 120,
  "words": 865012,
  "dir": "books/hongloumeng/",
  "index": "books/hongloumeng/README.md"
}
```

文件结构：

```
books/
  hongloumeng/            # 一本书一个目录
    README.md             #   目录页：书名、作者、简介、全部章回链接
    001.md … 120.md       #   每个文件一回，首行是回目
index.json                # 书目（slug / 作者 / 篇数 / 字数 / 目录路径）
LICENSE                   # 授权说明
```

## 授权

**正文**：均为公有领域作品（Public Domain），任何人可自由使用、复制、改编、商用，无需署名。

底本来自 [维基文库](https://zh.wikisource.org/) 等公开校本的整理，个别字词已做统一处理；校勘异文请以纸质权威版本为准。

**本仓库的整理工作**（分段、目录、JSON 结构、文件组织）以 [CC0 1.0](LICENSE) 释出。

## 不收录什么

在更的网文、出版社校注本、译注本**一律不收**——那些有版权，不是公有领域，放进公开仓库是侵权。

## 相关

- 站点：[baitaoshu.com](https://baitaoshu.com) — 793 本书在线阅读，含故事地图、听书、段落点评
- 项目主页：[baitaoshu.github.io](https://baitaoshu.github.io) · [仓库](https://github.com/baitaoshu/baitaoshu.github.io)
- 账号：[github.com/baitaoshu](https://github.com/baitaoshu)
