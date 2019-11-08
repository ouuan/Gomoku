# Gomoku

[Botzone 用户主页](https://botzone.org.cn/user/5db6b765d8a86373ab32ff5a)

Not So Naive ver.55 简介：

1. 动态计算每个空格对于双方的估价函数，使用 `std::set` 进行维护。估价函数基于下了这步棋后在四个方向上能连成的活/死一二三四五数量。

2. 每次挑选 max(黑棋估价, 白棋估价) 最大的若干个空格作为子节点，进行 min-max 对抗搜索，过程中使用 alpha-beta 剪枝。

若无法编译，请参阅 [Botzone 上的说明](https://wiki.botzone.org.cn/index.php?title=JSONCPP) 。