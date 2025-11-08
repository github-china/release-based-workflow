<!--
  <<< Author notes: Step 6 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 6: 提交一个热修复（hotfix）

_离完成就差一步啦 :heart:_
 
你可能注意到了，我并没有删除那个分支 —— 这是**有意为之**的。

在实际项目中，发版后发现问题的情况并不少见。为了能及时修复，我们通常会在同一个发布分支上直接提交补丁，而不是重新开始。

现在发布已完成，记得我们前面说过，我故意引入了一个 bug：本想只把文字颜色改为绿色，结果整个游戏背景都被改了。

_注意: GitHub Pages 更新有时需要几分钟，页面可能不会立刻显示你的最新改动。_

![image](https://user-images.githubusercontent.com/13326548/48045461-487dd800-e145-11e8-843c-b91a82213eb8.png)

这种快速修复软件中 bug 的操作，称为热修复（hotfix）。它是软件开发中的常规流程，你可能在其他App更新日志中经常见过类似描述：“修复了一些已知问题” —— 这通常就是热修复。

我们已为你创建好两个分支：

- `hotfix-v1.0.1`
- `fix-game-background`

接下来，我们将通过创建并合并 Pull Request 完成热修复：先合并到热修复分支，再同步到 main。

### :keyboard: 实操环节：创建并合并hotfix拉取请求

1. 创建一个新的拉取请求，选择 `base: hotfix-v1.0.1`，对比分支为 `compare: fix-game-background`。
2. 填写标题与描述。可以将标题设为 **Hotfix for broken game style**，描述如下：
   ```
   ## Description:
   - Fixed bug, set game background back to black
   ```
3. 检查修改内容，点击 **Create pull request**。
4. 点击 **Merge pull request**（合并拉取请求）将修复合并进 hotfix 分支。

现在，我们还需要把这次修复同步到主分支 `main`。

### :keyboard: 实操环节: 将热修复合并到主分支

1. 创建一个新的拉取请求，选择 `base: main`，对比分支为 `compare: hotfix-v1.0.1`。
2. 设置标题为 **Hotfix v1.0.1**。
   你可以参考以下示例描述：
   ```markdown
   ## Description:
   - Fixed bug introduced in last production release - set game background back to black
   ```
3. 检查修改内容，点击 **Create pull request**。
4. 点击 **Merge pull request** 完成合并。
5. 等待约 20 秒后刷新此页面，[GitHub Actions](https://docs.github.com/en/actions) 会自动检测并进入下一步。