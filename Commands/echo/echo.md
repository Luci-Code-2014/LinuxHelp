# echo

## 关于 **echo**

echo 是一个关于 **输出** 的命令, 参数有:

| 参数 | 意思 |
| --- | --- |
| -n | 去除自动换行 |
| -e | 启用反斜杠转义 |
| -E | 禁用反斜杠转义 (默认) |
| --help | 显示帮助信息 |
| --version | 显示版本 |

参数列表: echo <参数1 (可选, 使用上面的参数)> <字符串 (输出内容, 可选, 如果没有就是输出空行)>

## 示例

- 命令: `echo "HelloWorld"`
- 运行:
```
[root@archlinux: ~] # echo "HelloWorld"
HelloWorld
[root@archlinux: ~] # 
```

- 命令: `echo -n "Please input: "`
- 运行:
```
[root@archlinux: ~] # echo -n "HelloWorld"
Please input: [root@archlinux: ~] # 
```

- 命令: `echo -e "哦对了\n哦对了"`
- 运行:
```
[root@archlinux: ~] # echo -e "哦对了\n哦对了"
哦对了
哦对了
[root@archlinux: ~] # 
```

- 命令: `echo -E "哦对了\n哦对了"`
- 运行:
```
[root@archlinux: ~] # echo -E "哦对了\n哦对了"
哦对了\n哦对了
[root@archlinux: ~] # 
```