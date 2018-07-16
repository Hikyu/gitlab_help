# 基于分支进行review

源分支：**公共仓库中新建的分支**；
目的分支：**公共仓库的开发分支**。

Merge Request 流程如下：

1. 准备工作：

   - 项目成员将公共仓库项目 [clone](/setup/clone.md) 到本地；

   - **本地仓库开发分支**默认已经跟踪**公共仓库开发分支**

2. 提交代码：

   - 拉取**公共仓库开发分支**的内容，更新本地仓库开发分支；

   - **从本地仓库开发分支**创建临时分支并检出到新分支；

   - 针对需求或者 BUG，修改代码，推送临时分支到**公共仓库**（gitlab自动在公共仓库建立同名分支）；
   
   - 发起 [Merge Request](/review/local-modify.md)，请求合并**公共仓库临时分支**代码到**公共仓库开发分支**；

   - 项目组长[评审代码](/review/discuss.md)，进行讨论，最终评审通过，代码被项目组长合并到**公共仓库开发分支**；
   
![](/assets/branch-review.png)

> **[info] 注意**
>
> 创建分支、提交代码、提交 merger request等操作细节参考[](/review/fork/fork.md)这一章节，不再赘述。


