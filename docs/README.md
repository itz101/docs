## Personal Docs

### 部署方式

使用`gh-pages`工具：

```bash
npm install gh-pages --save-dev
```

Step: 将仓库克隆下来，（若`idoc`版本不匹配请先更新）直接进入`docs`目录下使用`npx idoc`，最后使用`npm run deploy`将`dist`文件部署至`gh-pages`分支，机器人将自动`deploy`。前提要在`package.json`文件内更新：

```json
"scripts": {
  "deploy": "gh-pages -d dist"
}
```



### Git高质量用法：

```bash
git log --graph --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%an%C(reset)%C(bold yellow)%d%C(reset) %C(dim white)- %s%C(reset)' --all
```

```bash
git subtree push --prefix=dist origin gh-pages
```

> 
