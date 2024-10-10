# leoatchina's tmux config
## 版本要求
tmux 3.0+,  之前作了很多兼容性配置，非常吃力不讨好，因此就把版本要求提高，低版本tmux直接退出。
可以通过 conda install -c conda-forge tmux 安装

## 安装
```
 ln -sf tmux.conf ~/.tmux.conf
```

## 主要操作
**注意**:
- 下面的`M`是指`Alt`
- `-`后面的字符有`大小写`之分
- `bind` 后面有 `-n` 是 `直接map`, 不需要再按先导键`M-o`

```
# 总体查看
M-o M-o (输入编号)

# 窗口操作
## 新建窗口
M-O

## 切换窗口
M-P (上一个窗口)
M-N (下一个窗口)

## 交换窗口位置并切换
Shift-Left  (与左边窗口交换位置并切换到左边窗口)
Shift-Right (与右边窗口交换位置并切换到右边窗口)

## 移动窗口到指定位置
M-o M-p (移动到左边)
M-o M-n (移动到右边)

## 切换到最后一个窗口
M-o Tab

## 关闭窗口
M-o M-q

## 移动窗口到指定编号
M-o Space (输入编号)

# panel操作
## 分割面板
M-] 水平分割
M-[ 垂直分割

## 选择面板
M-H 左
M-J 下
M-K 上
M-L 右

## 关闭面板
M-\ 关闭当前面板

## 交换面板位置
M-o [ 
M-o ]

## 调整面板大小
M-o M-h/M-j/M-k/M-l
```



