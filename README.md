# livenotes-site

用 [livenotes](https://github.com/) 构建脚本生成的学习笔记，托管在 GitHub Pages 上。

目录结构是 `<课程标识>/<内容分支>/`，比如 `U1__English__4/05__ai_english_quick/`——
不同课程底下经常有同名的内容分支文件夹（比如都叫 `05__ai_english_quick`），
所以前面要加一层课程标识区分开，不能直接把内容分支放根目录。根目录 `index.html` 是课程列表。

## 怎么发布新课程 / 更新内容

在 livenotes 项目里跑：

```
node build.js --src "<课程源目录>" --out "C:\Users\lmj_0\livenotes-site\<课程标识>\<内容分支文件夹名>"
```

然后在这个仓库里：

```
git add .
git commit -m "更新 <课程名>"
git push
```

新课程记得同时在根目录 `index.html` 里加一条链接。
