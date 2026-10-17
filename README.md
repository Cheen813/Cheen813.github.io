# 陈Cheeen 个人品牌站

纯静态单页网站（原生 HTML / CSS / JavaScript，零依赖），可部署到 GitHub Pages。

## 文件结构

```
site/
├── index.html          # 页面（全部样式与脚本都内嵌，改这一个文件即可）
└── assets/
    └── portrait.jpg    # 个人照片
```

## 一、在电脑上预览

**方式 A（最简单）**：直接双击 `site/index.html`，用浏览器打开即可。

**方式 B（本地服务器，效果更接近线上）**：
电脑装过 Python 的话，在 `site` 文件夹里打开终端，运行：

```bash
python -m http.server 8000
```

然后浏览器访问 `http://localhost:8000`。
按 `F12` 打开开发者工具 → 点设备图标（手机模拟），可预览手机宽度效果。

## 二、发布到 GitHub Pages（免费）

1. 登录 [github.com](https://github.com)，右上角 `+` → `New repository` 新建仓库
   - 名称随意（如 `chen-site`），选 Public，**不要**勾选 README。
2. 仓库页点 `uploading an existing file`，把 `site` 文件夹里的**所有文件**（`index.html` 和 `assets` 整个文件夹）拖进去，点 `Commit changes`。
3. 进仓库 `Settings` → 左侧 `Pages`：
   - `Source` 选 `Deploy from a branch`
   - `Branch` 选 `main`，目录选 `/ (root)`，点 `Save`。
4. 等 1-2 分钟，访问 `https://你的用户名.github.io/仓库名/` 即可上线。

> 更新内容：改完 `index.html` 后，在仓库里重新上传覆盖同名文件即可。

## 三、发布前必须补 / 必须确认

| 事项 | 位置 |
|---|---|
| **微信号**（已填：sxc1234567） | `index.html` 搜「sxc1234567」可替换，共四处 |
| **公司信息**：已按「不出现公司名、流水可披露」处理 | 案例区块 |
| 照片授权说明：页面仅使用你本人的照片，无第三方版权内容 | assets/portrait.jpg |
