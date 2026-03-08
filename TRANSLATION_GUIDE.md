# 翻译指南

## 当前状态

✅ GitHub 仓库已创建
✅ 原书 PDF 已上传
⏳ 待提取文本内容
⏳ 待翻译

## 提取 PDF 文本

由于系统限制，目前无法直接提取 PDF 文本。建议使用以下方法之一：

### 方法 1：在线工具
- https://www.ilovepdf.com/pdf_to_word
- https://smallpdf.com/pdf-to-word
- https://pdf2doc.com/

### 方法 2：本地工具
```bash
# Ubuntu/Debian
sudo apt install poppler-utils
pdftotext investing.for.programmers.pdf investing.for.programmers.txt

# macOS
brew install poppler
pdftotext investing.for.programmers.pdf investing.for.programmers.txt
```

### 方法 3：Python 脚本
```bash
pip install PyPDF2 pdfplumber
python extract_pdf.py
```

## 翻译流程

1. 提取 PDF 文本到 `.txt` 文件
2. 按章节分割文本
3. 使用 AI 工具翻译（推荐）：
   - ChatGPT/Claude
   - DeepL
   - Google Translate
4. 校对和润色
5. 提交到 GitHub

## AI 翻译提示词

```
请将以下英文内容翻译成中文，要求：
1. 保持技术术语的准确性
2. 语言通顺，符合中文阅读习惯
3. 保留原文的结构和格式
4. 对于专业术语，可在括号内标注原文

[文本内容]
```

## 文件结构

```
investing-for-programmers-zh/
├── README.md                 # 项目说明
├── TRANSLATION_GUIDE.md      # 翻译指南
├── investing.for.programmers.pdf  # 原书 PDF
├── chapters/                 # 翻译章节
│   ├── chapter-01.md
│   ├── chapter-02.md
│   └── ...
└── original/                 # 原文（提取后）
    ├── chapter-01.txt
    ├── chapter-02.txt
    └── ...
```

## 贡献者

欢迎加入翻译！

1. Star 本仓库
2. Fork 并创建翻译分支
3. 提交 Pull Request
4. 在贡献者列表中添加你的名字

## 许可证

待确认原书许可证。翻译完成后将标注合适的许可证。
