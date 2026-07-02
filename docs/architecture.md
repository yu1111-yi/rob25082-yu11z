# C++贪吃蛇架构设计文档
## 1. 技术栈
标准C++11 + Windows控制台API（conio.h、windows.h）

## 2. 模块化分层设计
1. 入口层 main.cpp：程序启动、游戏循环调度；
2. 实体层 Snake类：存储蛇坐标、长度、移动、增长逻辑；
3. 控制层 Game类：地图绘制、食物生成、碰撞检测、计分管理；

## 3. 文件结构说明
- main.cpp：程序入口，主循环；
- snake.h + snake.cpp：蛇实体类封装；
- game.h + game.cpp：游戏全局控制逻辑；

## 4. Git分支管理规范
- main：稳定可运行版本；
- feature/draw-map：地图绘制开发分支；
- feature/snake-move：蛇移动功能分支；
- feature/score：计分与重启分支；

## 5. 代码合并规则
所有功能开发必须新建feature分支，完成后提交PR，团队审核无误再合并到main分支。
