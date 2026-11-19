# 日语学习资源

在线阅读：[日语学习资源导航](https://tidb100.github.io/jlpt/)。

## 目录结构

```text
jlpt/
├── index.html              # 支持手机阅读的资源导航主页
├── README.md
└── word/
    ├── ja-gojuon.html       # 五十音记忆表
    ├── ja-sushi.html        # 东京寿司店日语
    ├── ja-numbers.html      # 日语数字与金额
    ├── ja-date.html         # 日语日期与时间
    ├── ja-color.html        # 日语颜色十词
    └── en-cafe.html         # 咖啡店英语（拓展学习）
```

六个学习页面存放于 `word/`，其中五个为日语主题，一个为咖啡店英语拓展主题。文件复制自 [tidb100/mojifree 的 sources 目录](https://github.com/tidb100/mojifree/tree/main/sources)，保留原文件名和内容。更新学习资料时，先检查同名文件内容，再同步更新导航主页和本说明。主页使用相对链接，适用于项目站点和本地打开。

## GitHub Pages 访问地址

- 项目主页：https://tidb100.github.io/jlpt/
- [五十音记忆表](https://tidb100.github.io/jlpt/word/ja-gojuon.html)
- [东京寿司店日语](https://tidb100.github.io/jlpt/word/ja-sushi.html)
- [日语数字与金额](https://tidb100.github.io/jlpt/word/ja-numbers.html)
- [日语日期与时间](https://tidb100.github.io/jlpt/word/ja-date.html)
- [日语颜色十词](https://tidb100.github.io/jlpt/word/ja-color.html)
- [咖啡店英语（拓展学习）](https://tidb100.github.io/jlpt/word/en-cafe.html)

`https://tidb100.github.io/` 是账号根站点，通常由 `tidb100.github.io` 仓库提供；本仓库 `jlpt` 对应 `/jlpt/` 项目路径。GitHub 仓库中的文件预览地址显示源代码，在线阅读请使用上面的 Pages 地址。

## 启用 GitHub Pages

1. 打开仓库 **Settings → Pages**。
2. 在 **Build and deployment → Source** 选择 **Deploy from a branch**。
3. 选择 **main** 分支和 **/ (root)** 目录，点击 **Save**。
4. 等待 **Actions** 中的 **pages build and deployment** 成功，然后访问项目主页。

这是纯静态 HTML 网站，无需安装依赖或构建命令。入口 `index.html` 位于仓库根目录，因此发布目录应选择根目录，而不是 `word/`。如果当前 Source 为 GitHub Actions，可改为上述分支发布方式；本仓库不提供自定义部署工作流。

若出现 404，请检查 Pages 是否已启用、发布分支及根目录是否正确，并确认最近一次部署成功。Pages 设置需要具有仓库管理权限的账号操作。
