# VALENCIA 瓦来西雅大辞典

![VALENCIA Logo](image/logo_img.png)

## 项目简介

VALENCIA（瓦来西雅）是一个虚构语言——**𣿅语**（Irelav）的在线词典项目。本项目提供了完整的词典查询、字母表、词缀表、时态表等功能，为𣿅语学习者提供全面的语言工具。

**版本：** 2.0.0\
**作者：** DornGames\
**语言：** 𣿅语 / 中文

## 功能特性

- 📚 **词典查询**：支持𣿅语-中文双向查询
- 🔤 **字母表**：完整的𣿅语字母表
- 📝 **词缀表**：词缀变化规则表
- ⏰ **时态表**：时态变化规则表
- 🎓 **学习资源**：提供考试听力材料和国歌等学习资源
- 🔍 **搜索功能**：强大的单词搜索功能
- 🌐 **多语言支持**：支持中𣿅互译

## 项目结构

```
Valencia Bangswp - V2/
├── index.html              # 主页（词典查询入口）
├── basicLang/              # 基础语言模块
│   ├── alphabet.html       # 字母表
│   ├── alphabetDetail.html # 字母表详情
│   ├── alphabetDetail.xlsx # 字母表数据
│   ├── bwbæzencl.html      # 词缀表
│   ├── bwbæzenclDetail.html # 词缀表详情
│   ├── bwbæzenclDetail.xlsx # 词缀表数据
│   ├── tondhæ.html         # 时态表
│   ├── tondhæDetail.html   # 时态表详情
│   ├── edusrc.html         # 学习资源
│   ├── search.html         # 搜索页面
│   └── translation.html    # 翻译工具
├── image/                  # 图片资源
│   ├── bg.png
│   ├── logo_img.png
│   ├── search_bg.jpg
│   ├── search_ui.png
│   └── 文字云3D_wenziyun.cn_.png
├── js/                     # JavaScript文件
│   ├── tools.js
│   └── wordData.js         # 单词数据
├── video/                  # 视频资源
│   └── antiqueIrelav-D1.mp4
└── README.md               # 项目说明
```

## 使用方法

1. 直接打开 `index.html` 文件即可使用
2. 在搜索框中输入拉丁字母进行查询
3. 点击导航栏按钮访问不同功能页面
4. 所有页面使用相对路径，支持离线使用

## 技术栈

- **HTML5**：页面结构
- **CSS3**：样式设计
- **JavaScript**：交互逻辑
- **Excel**：数据存储（xlsx格式）

## 开发信息

- **作者：** DornGames (@dornhub)
- **Box3Pro：** @DornGames
- **作者(Box3Pro)：** @云游de鸽者
- **版本：** 2.0.0
- **发布日期：** 2025

## 版权说明

所有内容纯属虚构，与现实无关，敬请理性看待。

**版权所有 © 2025 DornGames**

## 部署

本项目支持通过GitHub Actions自动部署到InfinityFree：

```yaml
name: Deploy to InfinityFree via FTP
on:
  push:
    branches:
      - main
jobs:
  ftp-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v4
      - name: FTP Deploy
        uses: SamKirkland/FTP-Deploy-Action@v4.3.5
        with:
          server: ${{ secrets.FTP_HOST }}
          username: ${{ secrets.FTP_USERNAME }}
          password: ${{ secrets.FTP_PASSWORD }}
          server-dir: ${{ secrets.FTP_TARGET_FOLDER }}
```

## 许可证

本项目为私有项目，版权所有。

## 链接

- [主站](https://dornhub.github.io)
- [GitHub](https://github.com/dornhub)
- [Box3Pro主页](https://dao3.fun/profile/50450184)

***

**注意：** 本项目所有内容均为虚构创作，不涉及任何现实政治、历史或文化实体。
