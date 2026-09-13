# 2026年秋学生课程网站

该目录面向学生提供课程信息与教学资料。首页为`index.html`，下载资料位于`files`。当前工作区的Git只跟踪该发布目录及必要的GitHub Pages配置，其他助教资料保留在本地。

目标仓库：`song17122328/cloud-ai-2026`。

GitHub Pages配置完成并部署成功后，网址为：

https://song17122328.github.io/cloud-ai-2026/

个人远程仓库已创建，当前文件和首次提交在本地准备。GitHub Pages公开提供页面，不具有学生身份验证功能。

## 首次发布

1. 使用当前工作区的`main`分支，将首次提交推送到`origin`：`https://github.com/song17122328/cloud-ai-2026.git`。
2. 打开个人仓库Settings → Pages，在Source中选择 **GitHub Actions**。
3. 仓库工作流`.github/workflows/pages.yml`仅发布`云计算所有资料/学生课程网站`，将其中的`index.html`作为网站首页。
4. 在Actions中查看 **Publish student course website** 的运行状态。若首次推送时Pages尚未启用，配置完成后使用 **Run workflow** 再运行一次。
5. 部署成功后，通过Pages设置页的Visit site访问课程网址。

网站仓库的目录结构与本地一致，首页由工作流发布到网站根路径。本站采用GitHub Actions发布，无需把本地首页移到仓库根目录。旧AISIGSJTU历史不作为新主分支的祖先提交。

## 目录内容

- `index.html`：学生首页，包含简介、教学进度、综合项目、考核与资料下载。
- `files/syllabus-2026.pdf`：本学期表格版教学大纲。
- `files/grading-2026.pdf`：本学期10%／70%／20%评分细则。
- `files/lecture-01.pdf`至`lecture-07.pdf`：课程理论讲义。
- `files/llm-introduction.pdf`、`files/llm-topics.pdf`：大模型参考讲义。
- `.nojekyll`：按静态文件发布。

本目录不包含学生名单、成绩记录、助教内部手册、PPT修改清单或平台账号信息。未完成定稿的项目Notebook和实操讲义暂不纳入网站下载列表。

## 资料副本说明

网站中的第一讲副本排除了原PDF第2—3页的往年人员、考核和进度内容；大模型基础副本排除了原PDF第2页的往年综述作业要求。其他理论页面保留原内容，研究案例沿用其标注年份。源资料未被修改。

网站首页、2026教学大纲与评分细则用于本学期课程规则。原始PPT经手动修改后，使用更新的PDF替换对应下载文件，届时可采用修订后的完整讲义。

## 后续更新

修改`index.html`中的课程内容、进度或链接，将修订后的PDF放入`files/`。沿用文件名时，首页链接无需修改。完成后提交并推送`main`，工作流重新发布学生网站。

工作区根目录`.gitignore`按明确文件名单跟踪当前11份学生PDF。新增资料时，核对发布内容、更新首页链接，并在根目录`.gitignore`增加相应允许条目。内部手册、学生名单、评分记录和PPT源文件不加入跟踪范围。

Canvas通知、精确截止日期和作业提交仍由各教学班分别维护。学生网站链接可同时放入两门课程的Canvas首页。

官方说明：[创建GitHub Pages站点](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)、[配置发布源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。
