# Brainfuck语言

## 简介
在1993年，Urban Müller 发明了 Brainfuck 语言。这门语言可以说是编程语言界的 helloworld 了,它一共只含有 8 个有效字符，每个有效字符就是一条指令。语言虽然极致轻量，它却是一门图灵完备的编程语言。

## 文档
\> 指针向右移动一格
\< 指针向左移动一格 
\+ 使指针当前格数值加一 
\- 使指针当前格数值减一 
\. 把当前格数值按 ASCII 表输出到终端 
\, 从终端接受一 byte 的数据，存储其 ASCII 数值到当前格 
\[ 当指针当前值为 0 时，程序跳转至与之对应的 ] 之后；否则程序正常执行 
] 程序跳转回与之对应的 [ 处

## 例子

1. 在屏幕上打印A
```
+++++
[
  >+++++++++++++
  <-
]
>.
```

2. 在屏幕上打印Hello Word!：

```
++++++++++[>+++++++>++++++++++>+++>+<<<<-]>++.>+.+++++++..+++.>++.<<+++++++++++++++.>.+++.------.--------.>+.>.
```