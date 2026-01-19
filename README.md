# leoatchina's tmux config

## 版本要求
tmux 3.0+，之前作了很多兼容性配置，非常吃力不讨好，因此就把版本要求提高，低版本tmux直接退出。
可以通过 `conda install -c conda-forge tmux` 安装

## 安装
```bash
ln -sf tmux.conf ~/.tmux.conf
```

## 基本说明
- `M` 是指 `Alt` 键，格式为 `<Alt-x>`
- 前导键为 `<Alt-o>`
- 注意大小写区分, `<Alt-o>` 和 `<Alt-O>` 是不一样的
- `bind` 后面有 `-n` 是直接映射，不需要再按前导键

## 常用操作

### 分割面板
- `<Alt-]>` 水平分割
- `<Alt-[>` 垂直分割

### 新建窗口
- `<Alt-O>` 新建窗口

### 关闭
- `<Alt-\>` 关闭当前面板
- `<Alt-o> <Alt-q>` 关闭当前窗口
    - 一个窗口里有很多面板

### 跳转面板
- `<Alt-H>` 左
- `<Alt-J>` 下
- `<Alt-K>` 上
- `<Alt-L>` 右

### 切换窗口
- `<Alt-P>` 上一个窗口
- `<Alt-N>` 下一个窗口
- `<Alt-o> <Alt-w>` 切换到最后一个窗口
- `<Alt-o> <Tab>` 选择面板

### 调整面板大小
- `<Alt-o> <Alt-h>` 向左调整
- `<Alt-o> <Alt-j>` 向下调整
- `<Alt-o> <Alt-k>` 向上调整
- `<Alt-o> <Alt-l>` 向右调整

## 其他操作

### 交换窗口位置并切换
- `<Shift-Left>` 与左边窗口交换位置并切换到左边窗口
- `<Shift-Right>` 与右边窗口交换位置并切换到右边窗口

### 移动窗口到指定位置
- `<Alt-o> <Alt-p>` 移动到左边
- `<Alt-o> <Alt-n>` 移动到右边

### 移动窗口到指定编号
- `<Alt-o> <Space>` 输入编号

### 交换面板位置
- `<Alt-o> [` 与上面面板交换
- `<Alt-o> ]` 与下面面板交换

### 复制模式
- `<Alt-|>` 进入复制模式
- 复制模式下按 `v` 开始选择，`y` 复制，`<Enter>` 复制到系统剪贴板

### 重命名
- `<Alt-o> <Alt-s>` 重命名会话
- `<Alt-o> <Alt-r>` 重命名窗口

### 会话管理
- `tmux` 新建会话
- `tmux attach` 重新连接最近会话
- `tmux attach -t <name>` 连接指定会话
- `tmux detach` 或 `<Alt-o>d` 分离当前会话
- `<Alt-o> <Alt-o>` 选择面板（需安装 tmux-fzf）

### 配置重载
- `<Alt-o><Enter>` 重新加载配置文件
