# github

## github 加速

watt toolkit

## github 汉化

篡改猴

## github desktop 桌面客户端

## git LFS 大文件管理

## git fork

sync fork 同步

# github actions 自动化构建 github pages 自动化部署流程

```js
1：git push 后会发生什么？
本地 → GitHub 仓库（main 分支）
 ↓
GitHub 检测到 .github/workflows/deploy.yml
  ↓
触发 Actions 工作流（自动）

2：Actions 工作流
GitHub 创建一个 Ubuntu 虚拟机（Runner）
    ↓
依次执行 deploy.yml 中的 7 个 step
    ↓
约 1-3 分钟执行完成

3：GitHub Pages 部署上线
```

## git Actions ？？

git 的自动化流式线 CI/CD
https://github.com/actions
工作流成功后，GitHub Pages 会：

接收 Actions 上传的 dist/ artifact
把内容发布到 https://zhushukun.github.io/mybob/
在 Pages 设置页面显示：

4：访问 https://zhushukun.github.io/mybob/

## github pages
