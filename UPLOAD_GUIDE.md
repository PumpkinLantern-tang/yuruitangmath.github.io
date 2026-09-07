# Yurui Tang 个人主页上传说明

此文件包对应网站：https://yuruitangmath.github.io/

## 一、你已经拿到什么

- `index.html`：完整英文主页，含个人信息、研究兴趣、2 篇已发表论文及 8 篇未发表论文。
- `papers/`：10 篇 PDF，已改为简短英文文件名，并与网页中的每个 PDF 链接对应。
- `.nojekyll`：告诉 GitHub Pages 直接发布静态文件。它是空文件；部分电脑会默认隐藏它。
- `UPLOAD_GUIDE.md`：本说明，可以留在电脑，不必上传。

页面样式和所有正文都在 index.html 中。论文使用 HTML 原生 details/summary 展开摘要，公式使用普通 HTML/Unicode 和原生 MathML。无需安装软件、运行命令或另外上传 CSS、JavaScript、字体、照片；在现代浏览器中双击 index.html 即可本地预览。

## 二、上传到已有 GitHub 仓库

1. 下载完整压缩包并解压。
2. 登录 GitHub，打开你的主页仓库：
   https://github.com/yuruitangmath/yuruitangmath.github.io
3. 进入仓库的 **Code** 页面，选择要用于发布的分支（通常为 main）。回到仓库根目录，即打开仓库后看到 README 等文件的那一层。
4. 点击 **Add file → Upload files**。
5. 把解压后的 **index.html 文件**和整个 **papers 文件夹**一起拖入上传区。能看到 `.nojekyll` 时也一并上传。不要上传 ZIP 文件本身，也不要把包含它们的外层文件夹拖进去。
6. 确认上传列表里主页路径是 `index.html`，PDF 路径形如 `papers/nonhamiltonian-regular-sublinear-expanders.pdf`。如果变成 `yurui-tang-homepage/index.html`，说明多套了一层文件夹，需要退回重选。
7. 在页面底部填写提交说明，例如 `Update profile and ten papers`，选择直接提交到当前发布分支，然后点击 **Commit changes**。上传相同路径的 index.html 会更新原文件，不需要先删除整个仓库。

若浏览器没有保留拖入的文件夹：先上传 index.html；再在仓库根目录通过 **Add file → Create new file**，文件名填写 `papers/README.md`，内容填写 `Paper PDFs` 并提交。GitHub 会创建 papers 文件夹。进入它后，通过 **Add file → Upload files** 上传解压后 papers 文件夹里的 10 个 PDF。

若电脑隐藏了 `.nojekyll`：在仓库根目录点击 **Add file → Create new file**，输入 `.nojekyll`，在正文区域输入一个空格并提交即可。不要把它命名为 `.nojekyll.txt`。这是推荐的静态发布配置。

## 三、确认 GitHub Pages 设置

若原网站已经从 main 分支根目录正常发布，而且本次仍上传到同一位置，不需要重新配置。否则：

1. 仓库 **Settings → Pages**。
2. 在 **Build and deployment** 下，设置 **Source = Deploy from a branch**。
3. **Branch = main**（或你实际上传的分支），旁边目录选 **/(root)**。
4. 点击 **Save**。

不需要选择主题或配置自定义域名。此网站使用现有的 github.io 地址。

## 四、发布后验证

1. 打开仓库 **Actions**，等待最新的 Pages 构建/部署任务成功。GitHub 官方说明更新发布可能需要最多约 10 分钟。
2. 在浏览器地址栏直接输入 https://yuruitangmath.github.io/ ，不要把它当搜索关键词搜索。
3. 点击任意论文标题，应展开 Abstract，以及 PDF 或 arXiv/Journal 链接。
4. 点击 PDF，应该打开对应论文；例如：
   https://yuruitangmath.github.io/papers/nonhamiltonian-regular-sublinear-expanders.pdf
5. 如果看到旧页面，在 Mac 上按 Command + Shift + R，在 Windows/Linux 上按 Ctrl + F5，或者使用无痕窗口打开。

## 五、常见问题

| 现象 | 要检查的内容 |
| --- | --- |
| 首页 404 | 仓库名是否为 yuruitangmath.github.io；是否上传至已设置的发布分支；index.html 是否在发布目录的最外层；Actions 是否部署成功。 |
| 首页正常，但 PDF 404 | papers 文件夹是否上传；PDF 文件名、大小写和扩展名是否与下表完全一致；是否出现了 papers/papers 的重复目录。 |
| 更新后仍是旧网页 | 是否 Commit changes；是否部署完成；是否刷新缓存。 |
| 只有下载按钮，没有网页 | 是否仅上传 ZIP；是否错误命名为 index.html.txt；是否把 index.html 放在 ZIP 解压出的外层文件夹下。 |
| 在 Google/Bing 搜索不到 | 搜索引擎收录与 GitHub Pages 发布是不同的事情。先用网站完整地址直接访问来判断是否成功。 |

## 六、论文分类及 PDF 文件名

已发表论文按正式卷期年份分类：两篇均为 2026 年，虽然都在 2025 年在线发表。预印本按上一份清单保留 2026、2025 年各 4 篇。大团版本 Erdős–Sós 猜想的附件没有 arXiv 编号，目前保留 Manuscript, 2026 和本地 PDF 链接；其 2026 年归类沿用之前的主页清单。

| 分类 | 年份 | 论文 | papers 文件夹中的文件名 |
| --- | --- | --- | --- |
| 已发表 | 2026 | The maximum number of cliques in graphs with given fractional matching number and minimum degree | `fractional-matching-cliques.pdf` |
| 已发表 | 2026 | Sparse graphs with an independent or foresty minimum vertex cut | `sparse-graphs-minimum-vertex-cut.pdf` |
| 未发表 | 2026 | Nonhamiltonian regular sublinear expanders | `nonhamiltonian-regular-sublinear-expanders.pdf` |
| 未发表 | 2026 | Characterizing forbidden induced subgraphs that force top vertices to be Gallai vertices | `gallai-top-vertices-induced-subgraphs.pdf` |
| 未发表 | 2026 | Weakly pancyclic vertices in dense nonbipartite graphs | `weakly-pancyclic-vertices.pdf` |
| 未发表 | 2026 | On the large-clique version of the Erdős–Sós conjecture | `large-clique-erdos-sos.pdf` |
| 未发表 | 2025 | Extending two results on hamiltonian graphs involving the bipartite-hole-number | `hamiltonian-bipartite-hole-number.pdf` |
| 未发表 | 2025 | The circumference of a graph with given minimum degree and clique number | `circumference-minimum-degree-clique-number.pdf` |
| 未发表 | 2025 | Cycles and paths through vertices whose degrees are at least the bipartite-hole-number | `cycles-paths-bipartite-hole-number.pdf` |
| 未发表 | 2025 | The minimum size of a k-connected locally nonforesty graph | `k-connected-locally-nonforesty.pdf` |

## 七、以后如何修改

- **个人信息**：在 GitHub 点击 index.html，再点击铅笔按钮编辑。查找 `个人信息：在此修改`，即可修改姓名、Ph.D.、单位、邮箱及 ORCID；如果修改姓名，也应同步修改文件顶部 title 和 description。
- **论文内容**：搜索论文标题。每篇由 `<details class="paper-entry">` 开始、`</details>` 结束，标题、作者、期刊和 Abstract 均在该段内。用普通文本替换即可；正文中的小于号写为 `&lt;`，与号写为 `&amp;`。
- **更新同一篇 PDF**：保留本包规定的文件名，把新版 PDF 上传到同一个 papers 路径即可覆盖；主页链接不必改。
- **增加论文**：复制一整段 details，放入相应分类/年份中，修改内容、唯一 id、序号及链接，并同步更新页内数量；年份没有自动读取 PDF 的功能，新年份需复制一个 publication-year 分组。
- **论文正式发表**：把该条目从 Preprints 移到 Publications 对应卷期年份，改为 Published，填入期刊和 DOI，并更新两类的数量。
- **为大团论文增加 arXiv**：取得正式编号后，在该条目 paper-actions 中添加链接，例如 `<a class="paper-button" href="https://arxiv.org/abs/实际编号" target="_blank" rel="noopener noreferrer">arXiv</a>`，并在 venue 中补充编号。这里“实际编号”只是本说明中的占位文字；主页中没有伪造链接。

仅上传 PDF 不会自动生成论文条目。网页中新增论文和上传论文文件是两项独立操作。本包已经替你完成现有 10 篇的对应配置。

## 参考：GitHub 官方说明

- 发布目录：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- 快速开始与发布等待时间：https://docs.github.com/en/pages/quickstart
- 404 排查：https://docs.github.com/en/pages/getting-started-with-github-pages/troubleshooting-404-errors-for-github-pages-sites
