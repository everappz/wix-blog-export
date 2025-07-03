# Wix Blog Export 📝➡️📦

**Export your Wix blog posts and convert them into clean, readable Markdown format using Python, Selenium, and OpenAI GPT.**  
Perfect for migrating content to static site generators like Hugo, Jekyll, or any Markdown-based platform.

---

## ✨ Features

- 🔍 Parses your Wix blog sitemap
- 🌐 Renders dynamic content using headless Chrome (Selenium)
- 🧽 Extracts only post content from `#content-wrapper`
- 🖼 Downloads and localizes all image assets
- 🤖 Uses OpenAI GPT to convert HTML to Markdown
- 📦 Outputs a clean folder per post: `_index.html`, `_index.md`, and local images

---

## 🚀 Quick Start

### 1. Clone the Repo

```bash
git clone https://github.com/everappz/wix-blog-export.git
cd wix-blog-export
```

### 2. Add Your OpenAI API Key

Create a file named `OPENAI_API_KEY.TXT` in the project root and paste your API key:

```txt
sk-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

### 3. Run the Exporter

```bash
bash fetch_blog_posts.sh
```

All converted posts will be saved in the `downloads/` folder.

---

## 📂 Output Structure

```
downloads/
  blog-post-folder/
    _index.html      ← Cleaned original HTML
    _index.md        ← Converted Markdown
    image1.jpg
    image2.png
```

---

## 🧠 Why This Project?

Wix uses JavaScript to render blog content, so basic scraping won't work.  
This tool:
- Automates page rendering with Selenium
- Uses OpenAI's LLM to intelligently convert content into semantic Markdown
- Works out-of-the-box with most static site generators

---

## 🛠 Technologies Used

- **Python 3**
- **Selenium + Chrome WebDriver**
- **BeautifulSoup**
- **OpenAI GPT-4o API**

---

## 🔐 Requirements

- Python 3.7+
- Google Chrome (installed)
- An OpenAI API key (GPT-4o access recommended)

---

## 🙌 Contribute

Found a bug? Got an improvement idea? PRs and Issues are welcome!  
Let’s make migrating away from Wix painless.

---

## 📄 License

MIT License

---

## 🌍 Related Projects

- [appkeywords.pro](https://appkeywords.pro) — Simple ASO optimization tool

