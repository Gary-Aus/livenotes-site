# livenotes-site

用 [livenotes](https://github.com/) 构建脚本生成的学习笔记，托管在 GitHub Pages 上。

每个课程一个子文件夹，根目录 `index.html` 是课程列表。

## 怎么发布新课程 / 更新内容

在 livenotes 项目里跑：

```
node build.js --src "<课程源目录>" --out "C:\Users\lmj_0\livenotes-site\<给这个课程起的文件夹名>"
```

然后在这个仓库里：

```
git add .
git commit -m "更新 <课程名>"
git push
```

新课程记得同时在根目录 `index.html` 里加一条链接。
