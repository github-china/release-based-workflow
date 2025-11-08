<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 3: 创建发布拉取请求（Release PR）

_干得漂亮！你刚刚成功添加了一个新功能（修改背景色） :smile:_

### 发布分支与 `main` 分支的关系

在版本发布流程中，**应该尽早创建发布分支与主分支（`main`）之间的拉取请求**。即使这个PR会保持打开状态一段时间也没关系。

一般来说，一个发布拉取请求（Release PR）应包含以下信息：

- 关联的 [Issue 引用](https://docs.github.com/en/articles/basic-writing-and-formatting-syntax/#mentioning-people-and-teams)，说明这个 PR 解决了哪些问题。
- 对本次提交的详细描述，说明包含了哪些变更。
- 使用 [@提及](https://docs.github.com/en/articles/basic-writing-and-formatting-syntax/#mentioning-people-and-teams) 通知负责审查的人员或团队。

为方便操作，我已经在仓库中添加了 **拉取请求模板**。
创建 PR 时，系统会自动填充一段默认文本，帮助你确认和填写关键信息。
如果不想使用模板内容，可以直接清空默认文本并写入自己的说明。

### :keyboard: 实操环节：创建发布拉取请求

接下来，我们将创建一个用于发布的拉取请求， 对比 `release-v1.0` 分支与 `main` 分支的差异。

1. 创建一个**新的拉取请求（Pull Request）**，`base: main` 以及 `compare: release-v1.0`。
2. 将标题填写为：`Release v1.0`。
3. 在正文中详细描述更新内容，例如：
   ```
   ## 说明:
   - 将页面背景色修改为黑色
   - 将游戏文字颜色修改为绿色
   ```
4. 点击 **Create pull request**（创建拉取请求）。
5. 等待约 20 秒后刷新此页面，[GitHub Actions](https://docs.github.com/en/actions) 会自动检测更新并进入下一步。