# leoatchina's tmux config
## 版本要求
tmux 3.0+,  之前作了很多兼容性配置，非常吃力不讨好，因此就把版本要求提高，低版本tmux直接退出。
可以通过 conda install -c conda-forge tmux 安装

## 安装
```
 ln -s leotmux/.tmux.conf ~/.tmux.conf
```
## 基本操作
- 先导键是Alt-b
  - 按下Alt-b后
  - hjkl 调整大小
  - Alt+hjkl panel 也是调整大小，幅度不一样
- Alt+n/p 翻页
- Alt+Shift+n/p 移动页面
- Alt+\插入新tab
- Alt+Shift+\ close当前tab
- Alt+] 左右分割， Alt+[ 上下分割
- Alt+Shift+hjkl panel 跳转，甚至可以跳到vim里去
## 高级操作部分
- Alt+Shift+b 显示buffer
- Alt+Shift+m 开始paste操作
