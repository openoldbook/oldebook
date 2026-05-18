# 参与贡献指南

感谢你关注 OldEbook 公版书库！

## 书籍收录标准

- ✅ 作者去世满 70 年（依据作者卒年计算）
- ✅ 民国时期出版（1912-1949）且作者去世满 70 年
- ✅ 明确标记为公有领域的古籍数字化资源
- ❌ 作者去世不满 70 年且未进入公有领域
- ❌ 现代出版社出版的有版权书籍

## 如何添加书籍

### 1. 准备书籍文件

- PDF 格式，尽量使用高清扫描版
- 文件命名格式：`书名_作者_出版年.pdf`
- 上传至网盘（百度/夸克/阿里/迅雷任一种或多种）

### 2. 添加元数据

在 `books/metadata.json` 中按以下格式添加条目：

```json
{
  "id": "unique-book-id",
  "title": "书名",
  "author": "作者名",
  "author_death_year": 1900,
  "publication_year": 1935,
  "pages": 320,
  "source": "国家图书馆·数字方志",
  "source_url": "https://...",
  "watermark": "国图数字方志水印",
  "reviewed": true,
  "review_date": "2026-05-18",
  "description": "简要内容介绍",
  "download": {
    "baidu": "https://pan.baidu.com/s/...",
    "quark": "https://pan.quark.cn/s/...",
    "aliyun": "https://www.alipan.com/o/...",
    "xunlei": "https://pan.xunlei.com/s/..."
  },
  "tags": ["古籍", "方志", "文学"]
}
```

### 3. 提交 Pull Request

- Fork 本仓库
- 在分支中添加书籍条目
- 提交 PR，注明书籍版权依据（作者卒年）
- 等待审核通过

## 审核流程

所有书籍在合并前需经过以下审核：

1. **版权核查**：确认作者去世满 70 年
2. **内容核查**：确认文件完整、可读
3. **来源标注**：确认已注明数字化来源机构

## 问题反馈

- 网盘链接失效 → 提交 [Issue](https://github.com/你的用户名/oldebook-archive/issues)
- 书籍信息错误 → 提交 Issue 或 PR
- 版权争议 → 提交 Issue，我们将在 7 个工作日内处理

---

感谢每一位贡献者让公版书籍触手可及 📚
