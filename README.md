# test
笔记
# 11月2日笔记

### . 写 Markdown 的第零步

我们写文本的时候大多写的是中文, 可是输入法在输中文时使用的标点为全角标点, 如 `，。？！（）【】：；“”`. 这些标点是不被 Markdown 所认可的, 也是无法转义的. 

我建议大家写 Markdown 的时候都用半角标点, 即英文标点, 如 `,.?!()[]:;""`. 且每个半角标点在文本使用时加上后置空格, 符合英文标点的书写规范, 也更加美观.

以微软自带输入法举例, 在使用中文输入法时按下 `Ctrl` + `.(这是个句号)`, 切换标点的全角与半角. 这样即可中文输入+半角标点.

### 1. 标题 [数个 "#" + 空格 前置]

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

标题会在目录与大纲分级显示, 可以跳转. 

在 Typora 中建议开启 `严格模式`, 即不应为 `#标题`, 应为 `# 标题`. 

应该要手动补上空格, 使得 Markdown 语法在其他文本编辑器上兼容. 

### 2. 强调 [用 "**" 或 "__" 包围]

```
**欢迎报考南京大学!** (我喜欢用这种)
__欢迎报考南京大学!__
```

或者选中想要强调的文字按下 `Ctrl` + `B`. 

E.G. 

**欢迎报考南京大学!**

### 3. 斜体 [用 "*" 或 "_" 包围]

```
*欢迎大佬来浇浇我各种知识* (我喜欢用这种)
_欢迎大佬来浇浇我各种知识_
```

或者选中想要强调的文字按下 `Ctrl` + `I`. 

E.G. 

*欢迎大佬来浇浇我各种知识*

(P.S. ***斜体并强调*** [用 "***" 或 "___" 包围])

### 4. 删除线 [用 "~~" 包围]

```
~~我宣布个事儿, 我是Sabiyary!~~
```

E.G. 

~~我宣布个事儿, 我是Sabiyary!~~

### 5. *高亮 [用 "==" 包围]

**(注意: 此为扩展语法)**

```
==我喜欢黄色, 也喜欢绿色==
```

E.G. 

==我喜欢黄色, 也喜欢绿色==

### 6. 代码 [用 "`" 包围]

```
`sudo rm -rf /*`
```

E.G. 

`sudo rm -rf /*` (没事别乱敲这个! )

~~"请输入管理员密码: (闪烁的光标)"~~

### 7. 代码块 [按三个 "`" 并敲回车]

````c
```
// 这里就可以开始输入你要的代码了
#include <stdio.h>
int mian() {
    print（“Hello, world!\n"）;
    retrun O;
}
``` // (这三个"`"文本编辑器会帮你自动补全 一般不用手动输)
````

(我之前都是用这个来展示各种语法的, 应该不用举例了吧)

要想显示行数的话, 一般要在 Typora 的设置里勾上这个显示行数的选项. 

代码块里可以选择语言, 其会根据语言来自动高亮各个语句. 在选择语言后, ` ``` ` 会变为 ` ```` ` + `对应语言`.

### 8. 引用 [">" + 空格 前置]

```
> 24岁, 是学生.
> > 学生特有的无处不在(恼)
```

引用是可以嵌套的!

E.G. 

> 24岁, 是学生.
>
> > 学生特有的无处不在(恼)

### 9. 无序列表 ["-" 或  "+" + 空格 前置]

```
- 一颗是枣树 (我喜欢用这种)
+ 另一颗还是枣树
* (其实这种也可以, 不过由于在 Typora 中很难单个输入, 故不常用)
```

三种前置符都可以, 敲回车会自动补全, 可在 Typora 设置中调整补全的符号, 敲回车后按下 `Tab` 会缩进一级. 

E.G. 

- 一颗是枣树
- 另一颗还是枣树

### 10. 有序列表 [数字 + "." + 空格 前置]

```
我来这里就为了三件事:
1. 公平
2. 公平
3. 还是tm的公平!
```

敲回车会自动补全, 敲回车后按下 `Tab` 会缩进一级. 

E.G. 

我来这里就为了三件事:

1. 公平
2. 公平

3. 还是tm的公平!

### 11. *上标 [用 "^" 包围]

**(注意: 此为扩展语法)**

```
C语言中int的上限是 2^31^ - 1 = 2147483647
```

E.G. 

C语言中 `int` 的上限是 2^31^ - 1 = 2147483647

### 12. *下标 [用 "~" 包围]

**(注意: 此为扩展语法)**

```
H~2~O 是剧毒的!
```

E.G. 

H~2~O 是剧毒的!

### 13. *注释 ["[^]" 后置]

**(注意: 此为扩展语法)**

```
> 今日我们相聚于此, 是为了学习 Markdown 的使用, 它的教程对于全体「观众」而言, 值得足足两个硬币的支持鼓励![^1]

[^1]: 沃兹·基·硕德 改编自「公鸡」普契涅拉.
```

需要在文末写上注释对应的内容

E.G. 

> 今日我们相聚于此, 是为了学习 Markdown 的使用, 它的教程对于全体「观众」而言, 值得足足两个硬币的支持鼓励![^1]

[^1]: 沃兹·基·硕德 改编自「公鸡」普契涅拉.

### 14. 链接 [常用 "[ ]" + "( )" 分别包围文本与链接]

**(注意: 文内跳转为扩展用法)**

```
[来看看我贫瘠的仓库罢](https://github.com/Sakiyary)
[基础教程: 12. 下标](#12. 下标 [用 "~" 包围])
```

支持网页链接与文内跳转, 按住 `Ctrl` 并 `单击鼠标左键` 即可跳转.

E.G. 

[来看看我贫瘠的仓库罢](https://github.com/Sakiyary)

[基础教程: 12. 下标](#12. 下标 [用 "~" 包围])

### 15. 任务列表 ["- [ ]" + 空格 前置]

```
TodoList:
- [ ] 刷B站
- [ ] 写代码
- [x] 起床
```

用 `x` 代替 `[ ]` 中的空格来勾选任务列表. 在 Typora 中可以直接用鼠标左键单击勾选框.

E.G. TodoList:

- [ ] 刷B站
- [ ] 写代码
- [x] 起床

### 16. 表格 [用 "|" 绘制表格边框]

```
| 学号 | 姓名  | 年龄 |
| :--- | :---: | ---: | (引号的位置代表着 左对齐, 居中, 右对齐)
|114514|田所|24|
|1919810|浩三|25|
```

第一行为表头, 并由第二行分割线决定对齐方式与长度, 第三行及之后即表格数据

E.G. 

| 学号    | 姓名 | 年龄 |
| :------ | :--: | ---: |
| 114514  | 田所 |   24 |
| 1919810 | 浩三 |   25 |

### 17. 图片 [直接拖进来或者复制粘贴]

```
![图片](图片的位置)
```

我还是会选择拖进来或者复制粘贴啦~ 在 Typora 的设置里也可以改图片的储存方式. 

### 18. 分割线 [按三个 "*" 或 "-" 或 "_" 并敲回车]

```
***
--- (我喜欢用这种)
___
// (其实按三个及以上都可以)
```

由于 `*` 与 `_` 均会自动补全, 所以我觉得 `-` 最为方便.

E.G. 

***

---






