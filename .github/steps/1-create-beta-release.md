<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: 创建 beta 版本发布

_欢迎来到 "Release-based workflow" 课程 :sparkle:_

### GitHub Flow 简介

[GitHub flow](https://guides.github.com/introduction/flow/) 是一种轻量、基于分支的开发流程。

![github-flow](https://user-images.githubusercontent.com/6351798/48032310-63842400-e114-11e8-8db0-06dc0504dcb5.png)

有些项目采用**持续部署（Continuous Deployment）**，每当主分支（`main`）上有新的提交时，就会自动生成一个新版本并发布。

但也有一些项目采用更稳健的发布策略，通过明确的版本号（Version）和正式发布（Release）来管理每次迭代。

### 版本（Version）是什么

版本代表软件的不同阶段或迭代，就像操作系统或应用程序的升级。
例如：

- 从 **Windows 8.1 → Windows 10**
- 从 **macOS High Sierra → macOS Mojave**

在版本迭代过程中，开发者会修改代码、修复问题、运行测试，并确保新功能不会带来新的缺陷。
当代码经过验证后，团队会为这一状态打上版本标签，并正式发布给用户使用。

### :keyboard: 实操环节：为当前代码库创建一个发布版本

在本步骤中，你将为当前代码库创建一个Release（发布版本）。

GitHub 的 Release 指向某个具体的提交（commit）。
Release 可以包含 Markdown 格式的发布说明（Release Notes）和附件（例如可执行程序或安装包）。

在正式使用 release-based 工作流程之前，我们先手动创建一个标签（tag）和发布版本：

1. 打开一个新的浏览器标签页，方便一边操作一边阅读本教程。
2. 打开仓库的 **Releases** 页面。
   * 提示：点击仓库顶部的 **Code** 标签页，在仓库简介下方的导航栏中找到 **Releases** 链接。
3. 点击 **Create a new release**（创建新发布）。
4. 在 **Tag version** 字段中输入版本号：`v0.9`，目标分支（*Target*）保持为 `main`。
5. 输入标题，例如 **First beta release**（首个 beta 版本），并可选地添加发布说明。
6. 勾选 **Set as a pre-release**，表示这是测试版（beta）。
7. 点击 **Publish release**（发布版本）。

### :keyboard: 实操环节：引入一个待修复的 Bug

为了在后续演示bug修复流程，我们现在先**故意制造一个 bug**。 系统已为你准备好一个分支：`update-text-colors`。接下来我们将为这个分支创建一个拉取请求（Pull Request）并合并。

1. 创建新的拉取请求，基线选择 `base: release-v1.0`，对比分支选择 `compare: update-text-colors`。
2. 设置标题为 **Updated game text style**。
   你可以在描述中添加如下内容：

   ```markdown
   ## Description:
   - Updated game text color to green
   ```
3. 点击 **Create pull request**（创建拉取请求）。
4. 点击 **Merge pull request** 合并该请求，并删除分支。
5. 等待大约 20 秒后刷新此页面，[GitHub Actions](https://docs.github.com/en/actions) 会自动检测并进入下一步。
