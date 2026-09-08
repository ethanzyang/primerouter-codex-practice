# Codex文件整理练习

[下载完整练习包 practice-v2.zip](https://github.com/ethanzyang/primerouter-codex-practice/releases/download/practice-2026-09-08-v2/practice-v2.zip) · [版本与附件](https://github.com/ethanzyang/primerouter-codex-practice/releases/tag/practice-2026-09-08-v2)

PrimeRouter运营助手制作。7份虚构练习文件，没有客户资料。目标是先看计划，再分类，并核对两份内容不同的同名文件。

先确认已具备Python 3.9或更新版本，练习目录所在文件系统支持硬链接。将完整练习包解压后，选择同时包含organize_files.py与example-folder的父目录作为Codex工作目录。

以下是调用已有脚本的建议步骤；本例已实际验证脚本命令，尚未逐条验证客户端对这些自然语言指令的执行。先输入：

```text
请先阅读这个目录里的organize_files.py，解释它会怎样处理example-folder。
只对example-folder运行预览，列出移动计划，先不要执行移动。
告诉我两份会议记录.txt会分别去哪，等我确认。
```

核对计划包含 `会议记录.txt -> documents/会议记录-1.txt`，原有 `documents/会议记录.txt` 保留。本练习从预览到执行保持目录文件不变；脚本每次运行都会重新计算计划，预览不会锁定计划。有文件变化就重新预览并确认。确认后输入：

```text
先检查练习目录没有变化；有变化就重新预览并等我确认。
目录保持不变时，运行这个脚本的--apply，再列出整理结果。
打开两份会议记录核对内容，不要改其他目录。
```

练习撤销：

```text
我没有修改练习文件。请运行这个脚本的--undo，核对所有文件回到原路径，内容与练习包一致。
```

脚本按文件扩展名分类，只处理指定目录顶层；不是按文件语义自动理解。本例7份文件中移动6份，已有的documents/会议记录.txt原位保留。撤销保留空目录；撤销前检查本次移动文件和原路径，本次移动文件内容改变或原名被占用会停止，不监视目录里的所有文件。这里的指令用于调用已有脚本，不能据此声称一句话生成了整理器。

尚未安装Codex可阅读PrimeRouter的B站教程：https://www.bilibili.com/opus/1245579230726586406 。PrimeRouter提供第三方API接入，非OpenAI官方，模型调用按量计费。
