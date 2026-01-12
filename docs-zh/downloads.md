---
title: 下载资源
---

下载 BMad Method 资源用于离线使用、AI 训练或集成。

## 源码包

| 文件 | 描述 |
|------|-------------|
| **[bmad-sources.zip](/downloads/bmad-sources.zip)** | 完整的 BMad 源文件 |
| **[bmad-prompts.zip](/downloads/bmad-prompts.zip)** | 仅包含智能体和流程提示 |

## LLM 优化文件

这些文件专为 AI 使用设计 - 非常适合加载到 Claude、ChatGPT 或任何 LLM 上下文窗口中。

| 文件 | 描述 | 使用场景 |
|------|-------------|----------|
| **[llms.txt](/llms.txt)** | 带摘要的文档索引 | 快速概览、导航 |
| **[llms-full.txt](/llms-full.txt)** | 完整文档拼接文件 | 全上下文加载 |

### LLM 使用方法

**Claude 项目:**
```
将 llms-full.txt 作为项目知识库上传
```

**ChatGPT:**
```
粘贴 llms.txt 用于导航，或按需使用 llms-full.txt 中的部分内容
```

**API 使用:**
```python
import requests
docs = requests.get("https://bmad-code-org.github.io/BMAD-METHOD/llms-full.txt").text
# 包含在系统提示或上下文中
```

## 安装选项

### NPM (推荐)

```bash
npx bmad-method@alpha install
```

## 版本信息

- **当前版本:** 参见 [更新日志](https://github.com/bmad-code-org/BMAD-METHOD/blob/main/CHANGELOG.md)
- **发布说明:** 在 [GitHub Releases](https://github.com/bmad-code-org/BMAD-METHOD/releases) 查看

## API 访问

通过编程方式访问 BMad 文档:

```bash
# 获取文档索引
curl https://bmad-code-org.github.io/BMAD-METHOD/llms.txt

# 获取完整文档
curl https://bmad-code-org.github.io/BMAD-METHOD/llms-full.txt
```

## 参与贡献

想要改进 BMad Method？请查看:

- [贡献指南](https://github.com/bmad-code-org/BMAD-METHOD/blob/main/CONTRIBUTING.md)
- [GitHub 仓库](https://github.com/bmad-code-org/BMAD-METHOD)

---
## 术语说明

- **LLM**: 大型语言模型 (Large Language Model)，如 Claude、ChatGPT 等
- **API**: 应用程序编程接口 (Application Programming Interface)
- **NPM**: Node 包管理器 (Node Package Manager)
