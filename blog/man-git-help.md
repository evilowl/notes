#通用 Git 命令 

Git 就是我们常说的命令套件 平台，这意味着您使用的主命令是 git，命令行的第一个参数表示您想运行的特定 Git 命令。 任何时候，只要运行不带任何参数的 git 就可以看到通用 Git 命令清单。

以下列出部分该清单： 

* **add** 向 Git 索引添加一个新文件。您必须提交该文件，以向 Git 存储库添加其内容。
* **branch** 使您能列出签出（check out）的分支，确定当前处理的分支，创建新分支，销毁已经创建或签出的本地分支副本。该命令不能切换到其他分支：使用 Git 的 checkout 命令实现。
* **checkout** 签出指定的分支或文件/目录。如果签出一个分支，则该分支将成为工作分支。如果指定一个特定文件或目录，则该文件或目录将更新以匹配当前签入工作分支目录的版本。您还可以使用该命令基于指定现有分支的可选跟踪更改新建一个分支。
* **commit** 记录 Git 索引中的文件和目录更改。指定想提交更改的文件和目录时，您可以使用 -a 选项将所有挂起更改添加到 Git 跟踪的文件，也可以使用 --interactive 选项选择希望一起提交的文件和目录更改。（如果处理的是几个涉及大量文件的不同任务，但又想一起提交某些更改，那么后者将非常有用。提交是对本地存储库执行的操作；如果使用远程中央存储库，那么必须使用 Git 的 push 命令将本地更改传输到远程存储库。）
* **diff** 显示本地文件与其他提交之间，或者两次不同提交的文件之间的不同之处。使用该命令时常常指定文件名，显示指定文件与提交到当前分支存储库的文件版本之间的不同之处。
* **fetch** 从另一个存储检索索引更新，指出已经创建的新标记，并提供有关已经提交到该存储库但尚未在本地显示的文件或目录更改的信息。然后，可以使用 git log 命令检测可用更改。要在 fetch 之后实际检索相关文件更改，您可以使用 git pull 或 git rebase 命令。
* **grep** 查询或显示当前分支中文件模式的匹配。该命令支持大部分您所喜爱的 GNU grep 选项。
* **log** 展示当前分支或当前分支中指定文件的提交日志信息。
* **merge** 将一个分支的更改合并到另一个。该命令提供一些选项，用于确定是否自动提交合并的更改，这使您能在实际接受这些更改之前了解合并的影响。
* **mv** 重命名 Git 当前跟踪的文件、目录或符号链接。
* **pull** 从另一个存储库检索索引更新，并将其合并到当前分支的文件或目录。
* **push** 使用本地索引和对象更改信息更新远程存储库。
* **rebase** 更新当前分支以匹配远程分支，修改尚未传输到远程分支的本地提交，使其适用于远程分支的当前状态。这是一个强大而危险的命令，因为它会根据需要重写命令以便合并。如果对远程存储库的更改频率和范围不大，可以使用 git pull 命令替代。
* **rm** 移除 Git 当前跟踪的文件、目录或符号链接。
* **stash** 临时将当前更改推入堆栈，并将当前签出返回到原始状态。git stash save 在本地堆栈中保存当前更改，git stash apply 检索并重新应用它们。如果您想 fetch 远程更改或者要在不永久提交进行中的更改的情况下执行 rebase，那么这将非常有用。
* **status** 展示当前分支的状态，指出尚未提交的更改、不会跟踪的文件等等。 所有 Git 命令都接受 --help 选项，这是一个常用的选项，可以获取任何命令的详细信息，查看每个命令接受的命令行选项清单等等。您还可以执行命令 git help command 获取有关任何 Git 命令的帮助。 有关 Git 命令的完整清单，请执行 man git 命令查看 Git 的在线参考信息。 
