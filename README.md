# REVIEW

评测仓库，专注于云服务器（VPS）与网络表现的图文记录，帮助读者快速了解不同线路与套餐的实际体验。所有文章以 Markdown 形式保存，并配有完整的测速、路由与解锁截图。

## 在线阅读
- GitHub Pages：<https://nxtrace.github.io/REVIEW/>
- 本地预览：直接在 Markdown 查看器或 VS Code 中打开 `reviews/*.md`。

## 仓库结构
- `reviews/`：按服务提供商与方案划分的评测文档。
- `assets/`：存放截图、拓扑图以及延迟监控等配图，建议与评测同名的子目录，方便 Markdown 使用相对路径引用。
- `LICENSE`：内容授权说明。

## 写作建议
1. 每篇评测使用 `reviews/<provider>-<region>-<plan>.md` 的命名方式。
2. Markdown 顶部列出核心参数（例如价格、套餐、计费模式），随后是路由、速度、解锁、性能等章节。
3. 插图使用相对路径引用 `assets/` 下的文件，便于 Github 阅读。
4. 如引用外部测速或监控链接，请在对应章节附上来源并注明「实时数据」或「历史数据」。

## 现有评测
- [Misaka.HKG.Opt](https://nxtrace.github.io/REVIEW/reviews/misaka-hkg-opt/)
- [Misaka.TPE.Opt](https://nxtrace.github.io/REVIEW/reviews/misaka-tpe-opt/)
- [xTom Tokyo EPYC Gen 2](https://nxtrace.github.io/REVIEW/reviews/xtom-tokyo-epyc-gen2/)

## 友情链接
- 古博：<https://www.gubo.org>
- LowendAFF：<https://lowendaff.com>
- 咸鱼博客：<https://www.bug.cy>
