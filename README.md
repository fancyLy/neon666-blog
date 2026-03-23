# neon666.xyz - 个人技术博客

这是一个使用 Hexo 静态网站生成器和 Butterfly 主题构建的个人技术博客。

## 项目特点

- 🚀 **快速部署**: 使用 GitHub Actions 自动构建和部署
- 🎨 **美观主题**: 采用 Butterfly 主题，响应式设计
- 📱 **移动友好**: 完美适配各种设备
- 🔧 **技术栈**: Hexo + Node.js + GitHub Pages

## 本地开发

### 环境要求
- Node.js 12.0 或更高版本
- Git

### 安装步骤
1. 克隆仓库：
   ```bash
   git clone https://github.com/fancyLy/neon666-blog.git
   cd neon666-blog
   ```

2. 安装依赖：
   ```bash
   npm install
   ```

3. 本地预览：
   ```bash
   hexo clean
   hexo generate
   hexo server
   ```
   然后在浏览器中访问 http://localhost:4000

## 部署

本项目使用 GitHub Actions 自动部署到 GitHub Pages：

1. 推送代码到 `master` 分支
2. GitHub Actions 会自动运行构建流程
3. 生成的静态文件会自动部署到 `gh-pages` 分支
4. 网站通过 GitHub Pages 提供服务

## 网站结构

```
neon666-blog/
├── source/           # 内容目录
│   ├── _posts/      # 博客文章
│   ├── about/       # 关于页面
│   └── CNAME        # 自定义域名
├── themes/          # 主题目录
│   └── butterfly/   # Butterfly 主题
├── _config.yml      # Hexo 主配置
├── _config.butterfly.yml  # Butterfly 主题配置
└── .github/workflows/deploy.yml  # GitHub Actions 工作流
```

## 自定义域名

网站使用自定义域名 `neon666.xyz`，通过以下方式配置：
1. 在 `source/CNAME` 文件中指定域名
2. 在域名注册商（阿里云）配置 DNS 解析到 GitHub Pages

## 添加新文章

1. 创建新的 Markdown 文件：
   ```bash
   hexo new "文章标题"
   ```

2. 编辑 `source/_posts/文章标题.md` 文件

3. 添加 Front-matter：
   ```yaml
   ---
   title: 文章标题
   date: 2026-03-24 00:00:00
   tags: [标签1, 标签2]
   categories: 分类
   ---
   ```

4. 编写文章内容

## 许可证

本项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。

## 联系方式

- 网站: https://neon666.xyz
- GitHub: https://github.com/fancyLy
- 博客: https://neon666.xyz