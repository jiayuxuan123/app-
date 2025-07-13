# 贡献指南 (Contribution Guide)

## 欢迎 (Welcome)

欢迎为 “App Hub” 贡献您的作品！ (Welcome to contribute to "App Hub"!)

本商店致力于收录任何酷炫、有趣、有用的应用和项目，不设类型限制。只要您的作品可以被展示，都欢迎您来分享。
(This store is dedicated to curating any cool, interesting, and useful apps and projects without any type restrictions. As long as your work can be showcased, you are welcome to share it.)

## 如何贡献 (How to Contribute)

贡献您的作品非常简单，您只需要修改一个文件：`data.js`。
(Contributing your work is simple, you only need to modify one file: `data.js`.)

### 1. 准备您的作品信息 (1. Prepare Your Project Information)

请收集以下关于您的作品的信息，稍后您将用它们来填写数据模板。
(Please gather the following information about your project, which you will use to fill out the data template.)

* **作品名称 (name)**
* **作品类型 (type)**: 请注明作品的类型，例如：`纯前端` (Front-end)、`全栈` (Full-stack)、`移动应用` (Mobile App)、`桌面应用` (Desktop App)、`小程序` (Mini Program) 等。
* **作品标语 (tagline)**：一句话介绍您的作品。 (A one-sentence description.)
* **作品描述 (description)**：详细描述作品的功能、特点、技术栈等。 (A detailed description of its features, highlights, tech stack, etc.)
* **作品Logo (logo_url)**：一个图片链接。 (An image link.)
* **作品截图 (screenshot_url)**：一个图片链接。 (An image link.)
* **在线体验链接 (demo_url)**：作品可在线访问的 URL 或下载链接。 (The online URL or download link for your project.)
* **源代码链接 (source_url)**：如果您的作品有公开的源代码，请提供链接（GitHub、Gitee 等）。此项为可选。 (If your project has public source code, please provide the link (GitHub, Gitee, etc.). This is optional.)
* **作者 (author)**：您的用户名、昵称或原作者的名称。 (Your username, nickname, or the original author's name.)
* **联系方式 (contact)**: 如果作者有联系方式或主页，可以放在这里。此项为可选。 (If the author has contact information or a homepage, you can put it here. This is optional.)

### 2. 填写数据模板 (2. Fill out the Data Template)

请将您的作品信息添加到 `data.js` 文件中的 `allAppsData` 数组里。
(Please add your project information to the `allAppsData` array in the `data.js` file.)

#### **作品数据模板 (Project Data Template)**

请复制以下模板，并用您的作品信息替换其中的内容。
(Please copy the template below and replace the content with your project information.)

**重要提示 (Important Note):**

* 请确保您的 `id` 是唯一的，建议使用英文，例如 `your-project-name-v1`。
    (Please ensure your `id` is unique. English is recommended, e.g., `your-project-name-v1`.)
* **在 `logo_url` 和 `screenshot_url` 字段，如果您没有图片，您可以留空（""）或提供一个文字占位符链接。**
    (In the `logo_url` and `screenshot_url` fields, if you don't have images, you can leave the link empty ("") or provide a text placeholder link.)
* **文字占位符链接示例 (Text Placeholder Link Examples):**
    * Logo: `https://via.placeholder.com/120x120?text=作品名称`
    * 截图: `https://via.placeholder.com/600x400?text=作品名称+截图`

```json
{
  "id": "您的作品唯一ID",
  "name": "您的作品名称",
  "type": "您的作品类型",
  "tagline": "一句话介绍您的作品",
  "description": "详细描述您的作品的功能、特点、技术栈等。",
  "logo_url": "您的作品Logo图片链接",
  "screenshot_url": "您的作品截图图片链接",
  "demo_url": "您的作品可在线体验的URL 或下载链接",
  "source_url": "您的作品源代码链接（可选）",
  "author": "您的用户名或昵称（原作者名称）",
  "date_added": "YYYY-MM-DD (例如: 2025-07-11)"
}


```json
{
  "id": "您的作品唯一ID",
  "name": "您的作品名称",
  "type": "您的作品类型",
  "tagline": "一句话介绍您的作品",
  "description": "详细描述您的作品的功能、特点、技术栈等。",
  "logo_url": "您的作品Logo图片链接（如果暂时没有，可以提供一个文字占位符链接）",
  "screenshot_url": "您的作品截图图片链接（如果暂时没有，可以提供一个文字占位符链接）",
  "demo_url": "您的作品可在线体验的URL 或下载链接",
  "source_url": "您的作品源代码链接（可选）",
  "author": "您的用户名或昵称（原作者名称）",
  "date_added": "YYYY-MM-DD (例如: 2025-07-11)"
}



