# ashesofhean 的博客

基于 [Hexo](https://hexo.io/) + [Butterfly](https://butterfly.js.org/) 搭建的个人博客，托管在 GitHub Pages。

在线地址：**[ashesofhean.github.io](https://ashesofhean.github.io)**

---

## 仓库结构

| 分支 | 内容 | 说明 |
|------|------|------|
| `main` | 编译后的静态网页 | GitHub Pages 自动部署 |
| `source` | Hexo 源码 | 文章、配置、主题 |

---

## 从零搭建

换新电脑后，拉取源码并安装依赖：

```bash
git clone -b source git@github.com:ashesofhean/ashesofhean.github.io.git
cd ashesofhean.github.io
npm install
```

---

## 写文章

```bash
# 新建文章
hexo new post "文章标题"

# 编辑 source/_posts/文章标题.md

# 本地预览
hexo server
# 打开 http://localhost:4000
```

---

## 发布上线

```bash
# 部署网站（更新 main 分支）
hexo clean && hexo deploy

# 备份源码（更新 source 分支）
git add .
git commit -m "更新文章"
git push origin source
```

---

## 目录说明

```
blog/
├── _config.yml              # Hexo 主配置
├── _config.butterfly.yml    # Butterfly 主题配置
├── source/
│   ├── _posts/              # ← 文章放这里
│   ├── about/               # 关于页面
│   └── images/              # 图片资源
├── themes/butterfly/        # 主题
└── public/                  # 生成的网页（不用管）
```

---

## 技术栈

- **框架**: [Hexo 7.3](https://hexo.io/)
- **主题**: [Butterfly 5.5](https://butterfly.js.org/)
- **托管**: [GitHub Pages](https://pages.github.com/)
