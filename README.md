# Chengcheng Xu — Academic Homepage (Jekyll)

## 文件结构

```
├── _config.yml          ← 全局配置（姓名、邮箱、链接）
├── _data/
│   ├── education.yml    ← 教育经历（改这个文件就行）
│   ├── papers.yml       ← 论文列表
│   ├── awards.yml       ← 获奖
│   ├── teaching.yml     ← 教学
│   └── service.yml      ← 审稿/学会
├── _includes/
│   ├── header.html      ← 顶部 Hero 区
│   └── nav.html         ← 导航栏
├── _layouts/
│   └── default.html     ← 页面模板
├── assets/css/
│   └── style.css        ← 样式表
├── index.html           ← 主页（Liquid 模板，自动读取 _data）
├── photo.jpg            ← 你的照片（自行添加）
└── Chengcheng_CV.pdf    ← 你的 CV（自行添加）
```

## 部署

1. 把整个文件夹内容上传到 `isNineveh.github.io` 仓库
2. GitHub Pages 已设为 main branch → 自动构建
3. 访问 https://isnineveh.github.io

## 日常更新

### 加一篇新论文
编辑 `_data/papers.yml`，在 `working:` 下添加：
```yaml
  - num: 3
    authors: "<strong>Chengcheng Xu</strong>, ..."
    title: "Your New Paper Title"
    status: "Under Review — MIS Quarterly"
```

### 加一个新奖项
编辑 `_data/awards.yml`，添加：
```yaml
- name: Best Paper Award, ICIS 2026
  year: 2026
```

### 加一门新课
编辑 `_data/teaching.yml`，在 `courses:` 下添加：
```yaml
    - name: "IS6001: New Course"
      semester: Fall 2026
```

### 改个人信息
编辑 `_config.yml` 里的 `author:` 部分。

**不需要碰 HTML / CSS / JavaScript。**
