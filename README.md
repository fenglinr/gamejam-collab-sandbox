# Game Jam 双人 Git 协作练习

这是一个独立的练习仓库，用于在开题前跑通 GitHub + Git LFS 协作。它没有可运行的游戏，不依赖 Godot、.NET SDK 或 Blender，不代表正式项目的模块设计。

## 从这里开始

请阅读 [双人练习指南](docs/双人练习指南.md)。两人各用自己的 GitHub 账号、自己的本地副本；同一人使用另一台电脑时也单独克隆。

初始化时已完成的检查与尚待双人实测的部分，见 [初始化验证记录](docs/初始化验证记录.md)。

```text
game/samples/PlayerSettings.cs  C# 文本样例，可练习代码差异
game/assets/audio/test-tone.wav 有效的短音频，由 Git LFS 保存，可练习资产交接与锁定
practice/you.txt                你修改的文件
practice/friend.txt             朋友修改的文件
practice/shared.txt             可选冲突练习使用的文件
art-source/                    以后放制作源文件；当前只有说明
docs/                          练习步骤与验收清单
```

## 练习规则

- `main` 保存已完成的练习；一个任务一个短期分支。
- 做完任务，更新到最新 `main` 并检查后，再通过 Pull Request 合并。
- 示例音频设为可锁定文件；先取锁，再修改，合并后解锁。锁在三台电脑之间同样适用，不只区分两个人。
- 不上传缓存、安装包或凭据；素材旁的 `.import` 与 `.uid` 要保留。
- 正式开题后可以新建正式仓库，复用经过验证的规则；练习文件不必进入游戏。
