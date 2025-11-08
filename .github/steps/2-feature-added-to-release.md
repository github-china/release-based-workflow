<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: 向发布分支添加新功能

_干得漂亮！你已经成功创建了 beta 版本 :heart:_


### 发布管理

在准备版本发布时，我们需要为团队建立一个清晰的工作流程，确保所有工作都能井然有序的开展。

管理发布有多种策略：

* 有的团队会使用**长期存在的分支**，例如根据环境分为 `production`、`dev` 和 `main`。
* 也有团队采用更简单的方式：只用功能分支（feature branch），一旦开发完毕后合并到主分支（main）发布版本，然后被删除。

其实，没有哪种策略一定更好。
关键在于**有意识地规划分支结构**，并尽量减少长期存在的分支数量。

在本练习中，你将使用 `release-v1.0` 分支，作为每个发布版本对应的长期分支。

### 受保护的分支

同 `main` 分支一样，你也可以对发布分支启用保护。这样可以防止被强制推送（force push）或误删。本仓库中，`release-v1.0` 已经默认配置为受保护分支。

### 添加新功能

一次正式发布通常包含多个小改动。接下来，我们先忽略之前添加的那个bug，我先为游戏增加几个小功能。

我们要做的改动是：

- 将页面背景色改为黑色；
- 同时把文字颜色调整为绿色（这部分我会帮你一起完成）。

### :keyboard: 实操环节：修改 `base.css`

1. 基于 `main` 分支创建一个新分支，新分支名字自己取。
2. 打开 `base.css` 文件，将 `body` 的样式修改如下：

   ```css
   body {
       background-color: black;
   }
   ```

   这会把页面背景改为黑色。
3. 创建一个新的拉取请求（Pull Request）
    - **base 分支**：`release-v1.0`
    - **compare 分支**：你刚创建的新分支
4. 按模板填写 PR 描述，说明你做了什么。
5. 点击 **Create pull request**（创建拉取请求）。

### 将新功能合并到 release 分支

即使采用发布分支的工作流，**GitHub Flow**依然是团队协作的重要基础。
为了保持分支简洁，建议每个功能或修复都使用**短期分支**来完成，并尽快合并。

你现在可以将这个 feature 分支合并到 release 分支中，以便之后更早地创建最终的发布拉取请求。

### :keyboard: 实操环节：合并拉取请求

1. 点击 **Merge pull request**（合并拉取请求），并删除该分支。
2. 等待大约 20 秒后刷新本页面，[GitHub Actions](https://docs.github.com/en/actions) 会自动检测更新并进入下一步。