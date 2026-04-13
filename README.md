# Henghui Du - Academic Homepage

🌐 **Live URL**: `https://CserDu.github.io/` (部署后)

## 📁 项目结构

```
homepage/
├── index.html          # 主页面
├── style.css           # 样式文件
├── script.js           # 交互脚本
├── README.md           # 说明文档
└── images/             # 图片目录
    ├── profile.jpg     # 个人照片（需要添加）
    ├── favicon.png     # 网站图标（需要添加）
    ├── crab.png        # 论文缩略图（可选）
    ├── crab_v2.png     # 论文缩略图（可选）
    ├── appo.png        # 论文缩略图（可选）
    ├── video_detective.png  # 论文缩略图（可选）
    ├── avqa.png        # 论文缩略图（可选）
    ├── ofm.png         # 论文缩略图（可选）
    └── avqa_cot.png    # 论文缩略图（可选）
```

## 🚀 部署到 GitHub Pages

### 方法一：直接作为 `username.github.io` 仓库

1. 在 GitHub 上创建名为 `CserDu.github.io` 的仓库
2. 将 `homepage/` 目录下的所有文件推送到仓库根目录：

```bash
cd homepage
git init
git add .
git commit -m "Initial commit: personal homepage"
git branch -M main
git remote add origin https://github.com/CserDu/CserDu.github.io.git
git push -u origin main
```

3. 在 GitHub 仓库 → Settings → Pages，选择 `main` 分支，`/ (root)` 目录
4. 几分钟后访问 `https://CserDu.github.io/`

### 方法二：使用现有仓库的 `gh-pages` 分支

```bash
# 在现有仓库中
git checkout -b gh-pages
# 将 homepage/ 下文件复制到仓库根目录
git add .
git commit -m "Deploy homepage"
git push origin gh-pages
```

## 📝 自定义修改指南

### 1. 添加个人照片
将你的照片放入 `images/profile.jpg`（建议 400x400px 正方形照片）

### 2. 添加论文缩略图
为每篇论文准备一张缩略图（建议 360x220px），放入 `images/` 目录

### 3. 修改论文链接
在 `index.html` 中搜索 `pub-link`，将 `href="#"` 替换为实际的论文/代码链接

### 4. 添加更多内容
- **新论文**：复制一个 `.pub-item` 块并修改内容
- **新新闻**：复制一个 `.news-item` 块并修改内容
- **新奖项**：复制一个 `.award-item` 块并修改内容

### 5. 访客统计（可选）
注册 [ClustrMaps](https://clustrmaps.com/) 获取访客地图代码，替换 footer 中的占位链接

## 🎨 设计特点

- ✅ **响应式设计** - 完美适配手机/平板/桌面
- ✅ **现代极简风格** - 参考学术主页最佳实践
- ✅ **毛玻璃导航栏** - 带有 blur 效果的固定导航
- ✅ **平滑滚动动画** - Intersection Observer 驱动
- ✅ **暗示性交互** - hover 效果提升体验
- ✅ **纯静态页面** - 无需后端，GitHub Pages 直接托管
- ✅ **SEO 友好** - 包含 meta 标签
