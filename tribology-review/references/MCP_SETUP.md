# MCP Server Configuration | MCP服务器配置

This guide provides detailed instructions for setting up and configuring MCP (Model Context Protocol) servers required for the tribology review skill.

本文档提供摩擦学综述技能所需的MCP（模型上下文协议）服务器的详细设置和配置说明。

---

## 1. Overview | 概述

### Required MCP Servers | 必需的MCP服务器

| Server | Purpose | Priority | Status |
|--------|---------|----------|--------|
| arxiv-mcp-server | Search and retrieve papers from ArXiv | Essential | [ ] |
| scholar-mcp-server | Google Scholar literature search | Essential | [ ] |
| zotero-mcp-server | Reference management, personal library | Recommended | [ ] |
| pubmed-mcp-server | Biomedical literature, clinical research | Recommended | [ ] |

### Optional MCP Servers | 可选的MCP服务器

| Server | Purpose | Priority |
|--------|---------|----------|
| crossref-mcp-server | DOI and metadata lookup | Optional |

---

## 2. ArXiv MCP Server | ArXiv MCP服务器

### 2.1 Installation | 安装

#### Prerequisites | 前置条件
- Node.js 18+ installed
- npm or yarn package manager
- Git for version control

#### Installation Steps | 安装步骤

**Method 1: npm global install | 方法1：npm全局安装**
```bash
# Install globally
npm install -g arxiv-mcp-server

# Verify installation
arxiv-mcp-server --version
```

**Method 2: From source | 方法2：从源码安装**
```bash
# Clone repository
git clone https://github.com/your-username/arxiv-mcp-server.git
cd arxiv-mcp-server

# Install dependencies
npm install

# Build
npm run build

# Link globally
npm link
```

**Method 3: Using pip | 方法3：使用pip**
```bash
pip install arxiv-mcp-server
```

### 2.2 Configuration | 配置

#### Claude Desktop Configuration | Claude桌面配置

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "arxiv": {
      "command": "npx",
      "args": ["-y", "arxiv-mcp-server"],
      "env": {}
    }
  }
}
```

#### Environment Variables | 环境变量

| Variable | Default | Description |
|----------|---------|-------------|
| ARXIV_MAX_RESULTS | 25 | Maximum results per search |
| ARXIV_SORT_BY | "submittedDate" | Sort results by |
| ARXIV_SORT_ORDER | "descending" | Sort order |

### 2.3 Usage | 使用

#### Available Tools | 可用工具

| Tool | Description | Parameters |
|------|-------------|------------|
| search_papers | Search arXiv for papers | query, categories, max_results, sort_by |
| download_paper | Download paper PDF | paper_id |
| read_paper | Read paper metadata and abstract | paper_id |

#### Example Usage | 使用示例

**Search for DLC coating papers**:
```bash
search_papers(
  query: "DLC coating tribology friction wear",
  categories: ["cond-mat.mtrl-sci", "physics.app-ph"],
  max_results: 50,
  sort_by: "submittedDate"
)
```

**Download specific paper**:
```bash
download_paper(paper_id: "2301.12345")
```

**Read paper details**:
```bash
read_paper(paper_id: "2301.12345")
```

### 2.4 Troubleshooting | 故障排除

| Issue | Solution |
|-------|----------|
| Connection timeout | Increase timeout in config |
| No results | Broaden search query |
| PDF download fails | Check network connection |
| Invalid paper ID | Verify arXiv ID format |

**Common Errors | 常见错误**:
```
Error: arXiv API rate limit exceeded
Solution: Wait 1 minute, reduce request frequency

Error: Invalid query format
Solution: Use only alphanumeric characters and spaces

Error: Paper not found
Solution: Verify arXiv ID (format: YYMM.NNNNN or YYMM.NNNNNvV)
```

---

## 3. Scholar MCP Server | Scholar MCP服务器

### 3.1 Installation | 安装

#### Prerequisites | 前置条件
- Python 3.8+
- pip
- Google account (for Scholar access)

#### Installation Steps | 安装步骤

**Method 1: pip install | 方法1：pip安装**
```bash
pip install scholar-mcp-server
```

**Method 2: From source | 方法2：从源码安装**
```bash
git clone https://github.com/your-username/scholar-mcp-server.git
cd scholar-mcp-server
pip install -e .
```

### 3.2 Configuration | 配置

#### Browser Setup | 浏览器设置

Scholar MCP requires Chrome or Chromium browser installed.

**Chrome installation | Chrome安装**:
```bash
# Windows (Chocolatey)
choco install googlechrome

# macOS (Homebrew)
brew install --cask google-chrome

# Linux
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

#### Claude Desktop Configuration | Claude桌面配置

```json
{
  "mcpServers": {
    "scholar": {
      "command": "python",
      "args": ["-m", "scholar_mcp_server"],
      "env": {
        "SCHOLAR_HEADLESS": "true",
        "SCHOLAR_TIMEOUT": "30"
      }
    }
  }
}
```

#### Environment Variables | 环境变量

| Variable | Default | Description |
|----------|---------|-------------|
| SCHOLAR_HEADLESS | true | Run browser in headless mode |
| SCHOLAR_TIMEOUT | 30 | Request timeout in seconds |
| SCHOLAR_USER_AGENT | - | Custom user agent string |

### 3.3 Usage | 使用

#### Available Tools | 可用工具

| Tool | Description | Parameters |
|------|-------------|------------|
| search | Search Google Scholar | query, num_results, start_year |
| get_paper_details | Get paper metadata | url or paper_id |
| get_citations | Get citation count | url or paper_id |
| get_related | Find related papers | url or paper_id |

#### Example Usage | 使用示例

**Search for tribology papers**:
```bash
search(
  query: "DLC coating friction coefficient review",
  num_results: 20,
  start_year: 2019
)
```

**Get paper details**:
```bash
get_paper_details(
  url: "https://scholar.google.com/scholar?q=DLC+coating+review"
)
```

**Check citations**:
```bash
get_citations(
  paper_id: "10.1016/j.triboint.2023.108234"
)
```

### 3.4 Troubleshooting | 故障排除

| Issue | Solution |
|-------|----------|
| Browser not launching | Verify Chrome installation |
| CAPTCHA challenge | Wait, try again later |
| Rate limiting | Reduce request frequency |
| Login required | Use personal Google account |

**Common Errors | 常见错误**:
```
Error: Browser not found
Solution: Install Chrome/Chromium

Error: CAPTCHA verification required
Solution: Access Scholar directly, complete CAPTCHA

Error: Timeout waiting for results
Solution: Increase timeout value
```

---

## 4. Zotero MCP Server | Zotero MCP服务器

### 4.1 Installation | 安装

**Method 1: pip install | 方法1：pip安装**
```bash
pip install zotero-mcp-server
```

**Method 2: From source | 方法2：从源码安装**
```bash
git clone https://github.com/your-username/zotero-mcp-server.git
cd zotero-mcp-server
pip install -e .
```

### 4.2 Configuration | 配置

#### API Key Setup | API密钥设置

1. Go to [zotero.org/settings/keys](https://www.zotero.org/settings/keys)
2. Create new private key with read/write permissions
3. Note your User ID from [zotero.org/settings](https://www.zotero.org/settings)

#### Claude Desktop Configuration | Claude桌面配置

```json
{
  "mcpServers": {
    "zotero": {
      "command": "python",
      "args": ["-m", "zotero_mcp_server"],
      "env": {
        "ZOTERO_API_KEY": "your-api-key",
        "ZOTERO_USER_ID": "your-user-id"
      }
    }
  }
}
```

#### Environment Variables | 环境变量

| Variable | Description | Required |
|----------|-------------|----------|
| ZOTERO_API_KEY | Your Zotero private key | Yes |
| ZOTERO_USER_ID | Your Zotero user ID | Yes |

### 4.3 Usage | 使用

#### Available Tools | 可用工具

| Tool | Description | Parameters |
|------|-------------|------------|
| zotero_search_items | Search your Zotero library | query, limit, start |
| zotero_get_item | Get item details | item_key |
| zotero_get_item_fulltext | Get full text/attachment | item_key |
| zotero_create_item | Add new item to library | item_data |
| zotero_get_collections | List all collections | - |
| zotero_search_collections | Search collections | query |

#### Example Usage | 使用示例

**Search your library | 搜索文献库**:
```bash
zotero_search_items(
  query: "DLC coating friction",
  limit: 20
)
```

**Get item details | 获取条目详情**:
```bash
zotero_get_item(item_key: "XXXXXXXX")
```

**Get full text | 获取全文**:
```bash
zotero_get_item_fulltext(item_key: "XXXXXXXX")
```

**Search collections | 搜索收藏夹**:
```bash
zotero_search_collections(query: "tribology")
```

### 4.4 Troubleshooting | 故障排除

| Issue | Solution |
|-------|----------|
| Authentication failed | Verify API key and User ID |
| Item not found | Check item_key format |
| Rate limiting | Reduce request frequency |
| Attachment access denied | Check API key permissions |

---

## 5. PubMed MCP Server | PubMed MCP服务器

### 5.1 Installation | 安装

**Method 1: pip install | 方法1：pip安装**
```bash
pip install pubmed-mcp-server
```

**Method 2: From source | 方法2：从源码安装**
```bash
git clone https://github.com/your-username/pubmed-mcp-server.git
cd pubmed-mcp-server
pip install -e .
```

### 5.2 Configuration | 配置

#### Claude Desktop Configuration | Claude桌面配置

```json
{
  "mcpServers": {
    "pubmed": {
      "command": "python",
      "args": ["-m", "pubmed_mcp_server"],
      "env": {
        "PUBMED_EMAIL": "your-email@example.com",
        "PUBMED_API_KEY": "your-api-key (optional)"
      }
    }
  }
}
```

#### Environment Variables | 环境变量

| Variable | Description | Required |
|----------|-------------|----------|
| PUBMED_EMAIL | Your email (NCBI requirement) | Yes |
| PUBMED_API_KEY | NCBI API key (optional) | No |

**Get NCBI API Key | 获取NCBI API密钥**:
1. Go to [ncbi.nlm.nih.gov/account](https://www.ncbi.nlm.nih.gov/account)
2. Navigate to "API keys" section
3. Create new API key

### 5.3 Usage | 使用

#### Available Tools | 可用工具

| Tool | Description | Parameters |
|------|-------------|------------|
| pubmed_search_articles | Search PubMed database | query, max_results, filters |
| pubmed_get_article_details | Get article metadata | pmid |
| pubmed_get_fulltext | Get full text link | pmid |
| pubmed_get_citations | Get citation count | pmid |
| pubmed_find_similar | Find similar articles | pmid |

#### Example Usage | 使用示例

**Search for articles | 搜索文献**:
```bash
pubmed_search_articles(
  query: "DLC coating tribology",
  max_results: 50,
  filters: {
    "date_range": "2019:2024",
    "article_type": "Review"
  }
)
```

**Get article details | 获取文章详情**:
```bash
pubmed_get_article_details(pmid: "12345678")
```

**Get full text | 获取全文链接**:
```bash
pubmed_get_fulltext(pmid: "12345678")
```

**Find similar articles | 查找相似文献**:
```bash
pubmed_find_similar(pmid: "12345678")
```

**Search with MeSH terms | 使用MeSH词搜索**:
```bash
pubmed_search_articles(
  query: '"Diamond-Like Carbon"[MeSH] AND "friction"[MeSH]',
  max_results: 30
)
```

### 5.4 Useful MeSH Terms | 常用MeSH词

| Topic | MeSH Term |
|-------|-----------|
| Tribology | "Friction"[MeSH], "Wear"[MeSH], "Lubrication"[MeSH] |
| DLC | "Diamond-Like Carbon"[MeSH] |
| Coatings | "Coated Materials, Biocompatible"[MeSH] |
| Hardness | "Hardness"[MeSH] |
| Materials Science | "Materials Science"[MeSH] |

### 5.5 Troubleshooting | 故障排除

| Issue | Solution |
|-------|----------|
| No results | Broaden search terms |
| Authentication error | Verify email is correct |
| Rate limiting | Add API key for higher limits |
| Invalid PMID | Verify PMID format (numbers only) |

---

## 6. Crossref MCP Server (Optional) | Crossref MCP服务器（可选）

### 6.1 Installation | 安装

```bash
pip install crossref-mcp-server
```

### 6.2 Usage | 使用

```bash
# Lookup DOI
crossref_lookup(doi: "10.1016/j.triboint.2023.108234")

# Search by title
crossref_search(query: "DLC coating review")
```

---

## 7. Complete Configuration Example | 完整配置示例

### claude_desktop_config.json | claude_desktop_config.json

```json
{
  "mcpServers": {
    "arxiv": {
      "command": "npx",
      "args": ["-y", "arxiv-mcp-server"],
      "env": {
        "ARXIV_MAX_RESULTS": "50",
        "ARXIV_SORT_BY": "submittedDate",
        "ARXIV_SORT_ORDER": "descending"
      }
    },
    "scholar": {
      "command": "python",
      "args": ["-m", "scholar_mcp_server"],
      "env": {
        "SCHOLAR_HEADLESS": "true",
        "SCHOLAR_TIMEOUT": "30"
      }
    },
    "zotero": {
      "command": "python",
      "args": ["-m", "zotero_mcp_server"],
      "env": {
        "ZOTERO_API_KEY": "your-api-key",
        "ZOTERO_USER_ID": "your-user-id"
      }
    },
    "pubmed": {
      "command": "python",
      "args": ["-m", "pubmed_mcp_server"],
      "env": {
        "PUBMED_EMAIL": "your-email@example.com",
        "PUBMED_API_KEY": "your-api-key (optional)"
      }
    }
  }
}
```

---

## 8. Verification | 验证

### Test ArXiv Server | 测试ArXiv服务器

```javascript
// Search for papers
const result = await search_papers({
  query: "DLC coating tribology",
  max_results: 5
});
console.log(result);
```

**Expected output | 预期输出**:
```
{
  total_results: 1234,
  papers: [
    {
      id: "2301.12345",
      title: "...",
      authors: ["..."],
      abstract: "...",
      published: "2023-01-15"
    }
  ]
}
```

### Test Scholar Server | 测试Scholar服务器

```javascript
// Search for papers
const result = await search({
  query: "DLC coating friction review",
  num_results: 5
});
console.log(result);
```

**Expected output | 预期输出**:
```
[
  {
    title: "...",
    authors: ["..."],
    journal: "...",
    year: 2023,
    citations: 45,
    url: "..."
  }
]
```

### Test PubMed Server | 测试PubMed服务器

```javascript
// Search for articles
const result = await pubmed_search_articles({
  query: "DLC coating friction",
  max_results: 5
});
console.log(result);
```

**Expected output | 预期输出**:
```
{
  total_count: 1234,
  articles: [
    {
      pmid: "12345678",
      title: "...",
      authors: ["..."],
      journal: "...",
      year: 2023,
      abstract: "..."
    }
  ]
}
```

### Test Zotero Server | 测试Zotero服务器

```javascript
// Search library
const result = await zotero_search_items({
  query: "DLC coating",
  limit: 5
});
console.log(result);
```

**Expected output | 预期输出**:
```
{
  total_results: 50,
  items: [
    {
      key: "XXXXXXXX",
      title: "...",
      creators: ["..."],
      date: "2023",
      itemType: "journalArticle"
    }
  ]
}
```

---

## 8. Security Considerations | 安全注意事项

### API Key Protection | API密钥保护

1. **Never commit keys to version control | 切勿将密钥提交到版本控制**
   ```bash
   # Add to .gitignore
   echo "*.json" >> .gitignore  # if containing keys
   ```

2. **Use environment variables | 使用环境变量**
   ```bash
   # Set environment variable
   export ZOTERO_API_KEY="your-key"
   ```

3. **Restrict file permissions | 限制文件权限**
   ```bash
   chmod 600 claude_desktop_config.json
   ```

### Rate Limiting | 速率限制

| Server | Requests/Minute | Recommended |
|--------|-----------------|-------------|
| arXiv | 1 | Use cached results |
| Scholar | 1-3 | Add delays between requests |
| PubMed | 3 (no key) / 10 (with key) | Add API key for higher limits |
| Zotero | 10 | Standard use |

---

## 9. Alternative: Web-Based Search | 替代方案：基于网络的搜索

If MCP servers are unavailable, use web search:

### Google Scholar Web Search | 谷歌学术网页搜索

```bash
# Use WebSearch tool
websearch(query: "DLC coating tribology review 2023")
```

### Direct Journal Search | 直接期刊搜索

| Journal | URL |
|---------|-----|
| Tribology International | sciencedirect.com/triboint |
| Wear | sciencedirect.com/wear |
| Surface & Coatings Technology | sciencedirect.com/surfcoattech |

---

## 10. Support | 支持

### Getting Help | 获取帮助

| Issue | Resource |
|-------|----------|
| ArXiv MCP issues | [GitHub Issues](https://github.com/arxiv-mcp-server/issues) |
| Scholar MCP issues | [GitHub Issues](https://github.com/scholar-mcp-server/issues) |
| General questions | Open an Issue |

### Documentation | 文档

| Resource | URL |
|----------|-----|
| ArXiv API docs | https://arxiv.org/help/api |
| Google Scholar help | https://scholar.google.com/intl/en/scholar/help.html |
| Zotero API docs | https://www.zotero.org/support/dev/web_api |

---

**See also | 参见**:
- [LITERATURE_SOURCES.md](LITERATURE_SOURCES.md) - Literature sources guide
- [WORKFLOW.md](WORKFLOW.md) - Complete workflow
