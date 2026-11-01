# Academic Homepage

A single-file academic personal homepage (pure static HTML), ready for GitHub Pages.

## Files

```
academic-homepage/
├── index.html        # 主页（所有内容都在这一个文件里）
├── assets/
│   └── photo.jpg     # 你的照片（可选，没有照片页面会显示占位图）
│   └── cv.pdf        # 你的 CV（可选，导航栏 CV 链接指向它）
└── README.md
```

## 如何发布到 GitHub Pages（3 步）

1. **创建仓库**
   - 在 GitHub 上新建一个仓库，命名为：`caierayu.github.io`
   - 这样主页地址就是 `https://caierayu.github.io`

2. **上传文件**
   - 把 `index.html` 上传到仓库根目录（可通过网页 Add file → Upload files，或 git push）
   - 把你的照片放到 `assets/photo.jpg`，CV 放到 `assets/cv.pdf`

3. **开启 Pages**
   - 仓库 → Settings → Pages → Source 选 `Deploy from a branch`，Branch 选 `main` / `(root)` → Save
   - 等 1-2 分钟，访问 `https://你的用户名.github.io` 即可

> 提示：也可以用任意仓库名（如 `homepage`），然后在 Settings → Pages 里开启，
> 地址会变成 `https://你的用户名.github.io/homepage/`。

## 需要修改的占位符（在 index.html 中搜索即可）

| 占位内容 | 位置 |
|---|---|
| `Your Name` | 页面标题、导航栏、Hero 标题、作者列表、页脚 |
| 单位/职位 | Hero 区 `affiliation` 段落 |
| 个人简介 | Hero 区 `bio` 段落 |
| 邮箱 | Hero 区 + Contact 区 |
| 社交链接 | `social` 区的 `YOUR_USERNAME` 等链接 |
| News | `#news` 区列表，最新消息放最上面 |
| 研究方向 | `#research` 区的 chips |
| 论文 | `#publications` 区，每个 `.pub` 块复制一份即可新增论文 |
| 审稿服务 | `#services` 区 |

## 新增一篇论文

复制 `#publications` 里任一 `.pub` 块，改标题、venue、作者、链接即可。
- `.me` 类会给自己的名字加粗下划线
- `.tag-oral` / `.tag-spotlight` 可给论文加 Oral/Spotlight 标签，不需要就删掉
