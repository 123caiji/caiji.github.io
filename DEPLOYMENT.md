# 部署说明

## 项目概述

这是一个现代化的个人主页项目，展示物联网安全工程师龙天彪的专业能力、项目经历和学术成果。

## 文件结构

```
├── index.html              # 主页面文件
├── styles.css              # 样式文件
├── script.js               # JavaScript交互功能
├── test-images.html        # 图片测试页面
├── package.json            # 项目配置
├── README.md               # 项目说明
├── DEPLOYMENT.md           # 部署说明（本文件）
├── assets/                 # 资源文件夹
│   └── images/            # 图片资源
│       ├── avatar/        # 头像图片
│       └── certificates/  # 证书图片
└── other directories...   # 其他目录
```

## 部署到GitHub Pages

### 方法一：直接推送到GitHub

1. **克隆仓库**
   ```bash
   git clone https://github.com/123caiji/123caiji.github.io.git
   cd 123caiji.github.io
   ```

2. **添加文件**
   - 将修改后的文件复制到仓库目录
   - 确保所有文件都在正确的位置

3. **提交并推送**
   ```bash
   git add .
   git commit -m "Update personal homepage"
   git push origin main
   ```

4. **启用GitHub Pages**
   - 进入GitHub仓库设置
   - 找到"Pages"部分
   - 选择源分支（通常是main）
   - 保存设置

5. **访问网站**
   - 等待几分钟后访问：https://123caiji.github.io

### 方法二：使用GitHub Actions自动部署

项目已配置自动部署，每次推送到main分支时会自动部署。

## 本地预览

### 使用Python
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

### 使用Node.js
```bash
# 安装serve
npm install -g serve

# 启动服务器
serve -s . -l 3000
```

### 使用PHP
```bash
php -S localhost:8000
```

## 自定义配置

### 修改个人信息

1. **编辑 `index.html`**
   - 修改姓名、职位、联系方式
   - 更新个人简介和研究领域
   - 添加或修改论文列表
   - 更新工作经历和获奖信息

2. **更新图片资源**
   - 替换 `assets/images/avatar/avatar.png` 为您的头像
   - 更新 `assets/images/certificates/` 目录下的证书图片
   - 确保图片文件名与HTML中的引用一致

3. **修改样式**
   - 编辑 `styles.css` 调整颜色主题
   - 修改字体、间距等样式
   - 调整响应式断点

### 颜色主题自定义

在 `styles.css` 中修改以下CSS变量：

```css
:root {
    --primary-color: #4f46e5;    /* 主色调 */
    --secondary-color: #7c3aed;  /* 辅助色 */
    --accent-color: #fbbf24;     /* 强调色 */
    --text-color: #1f2937;       /* 文字颜色 */
    --bg-color: #ffffff;         /* 背景颜色 */
}
```

## 功能特性

### 已实现功能
- ✅ 响应式设计（支持桌面、平板、手机）
- ✅ 平滑滚动导航
- ✅ 移动端汉堡菜单
- ✅ 滚动动画效果
- ✅ 数字计数动画
- ✅ 联系表单验证
- ✅ 图片懒加载和错误处理
- ✅ 回到顶部按钮
- ✅ 键盘导航支持
- ✅ 触摸手势支持
- ✅ 网络状态检测
- ✅ 性能监控

### 浏览器支持
- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+

## 性能优化

### 已实现的优化
- 图片预加载
- CSS和JavaScript压缩
- 字体预加载
- 滚动事件防抖
- 图片懒加载

### 建议的进一步优化
- 使用CDN加载外部资源
- 启用Gzip压缩
- 添加Service Worker缓存
- 优化图片格式（WebP）

## 故障排除

### 常见问题

1. **图片不显示**
   - 检查图片路径是否正确
   - 确保图片文件存在
   - 查看浏览器控制台错误信息

2. **样式不生效**
   - 检查CSS文件路径
   - 清除浏览器缓存
   - 验证CSS语法

3. **JavaScript功能异常**
   - 检查浏览器控制台错误
   - 确保JavaScript文件正确加载
   - 验证HTML结构

4. **GitHub Pages不更新**
   - 等待几分钟让GitHub处理
   - 检查仓库设置中的Pages配置
   - 清除浏览器缓存

### 调试工具

1. **浏览器开发者工具**
   - F12打开开发者工具
   - 查看Console、Network、Elements面板

2. **图片测试页面**
   - 访问 `test-images.html` 检查图片加载状态

3. **移动端测试**
   - 使用浏览器开发者工具的移动端模拟器
   - 在不同设备上测试

## 更新维护

### 定期更新内容
- 更新个人简介和经历
- 添加新的论文和项目
- 更新证书和获奖信息
- 保持联系方式最新

### 技术更新
- 定期检查依赖项更新
- 优化代码性能
- 添加新功能
- 修复bug

## 联系支持

如果您在使用过程中遇到问题：

1. 查看本文档的故障排除部分
2. 在GitHub上提交Issue
3. 联系项目维护者

---

**注意**: 请根据您的实际需求修改所有占位符内容，包括个人信息、照片和链接。

