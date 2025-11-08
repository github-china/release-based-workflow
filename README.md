<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

[English](https://github.com/skills/release-based-workflow) | 中文

> 本课程翻译自 Github Skills，全部课程请点击 [这里查看](https://www.github-zh.com/getting-started)

# 创建一个基于发布的工作流程

_掌握以 GitHub Flow 为基础的发布型工作流程（release based workflow）。_


</header>

<!--
  <<< Author notes: Course start >>>
  Include start button, a note about Actions minutes,
  and tell the learner why they should take the course.
-->

## Welcome

本课程我们将学习基于发布的（release-based）工作流程，该流程建立在 [GitHub Flow](https://guides.github.com/introduction/flow/) 的基础之上。
当团队采用这种工作流程时，GitHub 能让你更方便地协作、打包代码，并把项目的稳定版本发布给更多用户下载和使用。

> [GitHub Flow](https://guides.github.com/introduction/flow/) 是一种轻量级的、基于分支的开发工作流程，特别适用于持续部署的团队。
它通过要求团队创建新分支进行开发、提交代码、发起 Pull Request（用于代码评审和讨论），以及在合并到主分支后立即部署，从而实现持续且高速地发布和部署软件。

GitHub 的 “发布（release）” 功能，可以让你的团队基于项目历史中的某个节点，将软件打包并提供给用户使用。

- **适合人群**：开发者、DevOps 工程师、运维人员、管理者和开发团队。
- **你将学到**：如何按照发布为核心的工作流程开展项目。
- **你将构建**：创建标签（tag）、发布版本（release）和发布说明（release notes）。
- **学习前提**：如果你还不了解分支、提交和Pull Request，建议先学习 [GitHub 入门课程](https://github.com/github-china/introduction-to-github)。
- **课程时长**：不到 1 小时。

课程内容如下：

1. 创建 beta 测试版本
2. 向版本中添加新功能
3. 创建用于发布的拉取请求（Pull Request）
4. 添加发布说明并合并代码
5. 发布正式版本
6. 提交紧急修复（hotfix）
7. 创建修复后的发布版本

### 如何开始课程

<!-- For start course, run in JavaScript:
'https://github.com/new?' + new URLSearchParams({
  template_owner: 'skills',
  template_name: 'release-based-workflow',
  owner: '@me',
  name: 'skills-release-based-workflow',
  description: 'My clone repository',
  visibility: 'public',
}).toString()
-->

[![start-course](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=github-china&template_name=release-based-workflow&owner=%40me&name=skills-release-based-workflow&description=My+clone+repository&visibility=public)

1. 右键点击上方 **Start course** 按钮，选择在新标签页中打开链接。
2. 在新页面中根据系统提示新建一个仓库。
   - 仓库名称、描述这些字段系统已经帮我们自动填充好了，您可以按需修改。
   - 建议使用选择公开仓库，因为私有仓库有[GitHub Actions 分钟数限制](https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions)。
   - 最后点击 Create repository 按钮
3. 仓库创建完毕后，等待大约 20 秒（等待Action执行），然后刷新页面。注意是刷新您仓库的页面，不是本课程的页面。如果页面没有变化，请继续等待。然后按照 README 中的步骤一步步进行。

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/release-based-workflow) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
