<!--
  <<< Author notes: Step 4 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 4: 生成发布说明并完成合并

_你成功创建了一个 Release PR :dancer:_

### 自动生成发布说明

版本发布时我们一般需要填写发布说明，好让用户和团队成员快速了解本次更新包含了哪些新功能、修复了哪些问题，以及其他重要变更。 
GitHub提供了[自动生成发布说明](https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes)的功能，可以替代手动编写发布说明。 
通过它，你能快速生成一个版本更新概览，其中包括：

* 已合并的拉取请求列表
* 本次发布的贡献者名单
* 完整变更日志的链接

生成后，你也可以根据需要对内容进行自定义修改。

### :keyboard: 实操环节：生成发布说明

1. 打开一个新的浏览器标签页，进入当前仓库的 **Releases** 页面。
   - 提示：点击仓库顶部的 **Code** 标签页，然后在仓库描述下方的导航栏中，点击 **Releases** 链接即可进入。
2. 点击 **Draft a new release**（创建新发布草稿）。
3. 在 *Tag version* 输入框中填写 `v1.0.0`。
4. 在标签右侧的 *Target* 下拉菜单中，选择分支 `release-v1.0`。
   - *提示：这是临时设置，用于基于该分支的变更生成发布说明。*
5. 在描述框右上角点击 **Generate release notes**（生成发布说明）。
6. 查看自动生成的发布说明，如有需要可在文本框中自行调整内容。
7. 将 *Target* 分支改回 `main`，因为最终发布的标签应创建在主分支上。
8. 点击 **Save draft**（保存草稿），稍后我们会正式发布该版本。

现在你可以[合并](https://docs.github.com/en/get-started/quickstart/github-glossary#merge)你的拉取请求啦！

### :keyboard: 实操环节：合并到主分支

1. 打开一个新的标签页，进入仓库的 **Pull requests** 页面。
2. 找到并打开你之前创建的 **Release v1.0** 拉取请求。
3. 点击 **Merge pull request**（合并拉取请求）。
4. 等待大约 20 秒，然后刷新本页。[GitHub Actions](https://docs.github.com/en/actions) 将自动检测进度并进入下一步。
