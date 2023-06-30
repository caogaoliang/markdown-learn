# markdown-learn

***Author ：caogaoliang***   
*date : 2023 / 06*

[toc]

## 一. 标题

```Markdown
格式: # + 空格 + 标题内容 (建议标题的前后都要空1行)
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

---

## 二. 文本字体

```Markdown
*斜体字体*
**粗体字体**
***粗斜体字体***
```

*斜体字体*
**粗体字体**
***粗斜体字体***

---

## 三. 列表

```Markdown
无序列表的格式: - + 空格 + 列表内容
- 无序列表 1
    - 无序列表 1.1
- 无序列表 2
    - 无序列表 2.1
    - 无序列表 2.2
        - 无序列表 2.2.1
```

- 无序列表 1
    - 无序列表 1.1
- 无序列表 2
    - 无序列表 2.1
    - 无序列表 2.2
        - 无序列表 2.2.1

---

```Markdown
有序列表的格式: 数字序号 + 英文句号 + 空格 + 列表内容
1. 有序列表 1
    1. 有序列表 1.1
2. 有序列表 2
3. 有序列表 3
    1. 有序列表 3.1
    2. 有序列表 3.2
```
1. 有序列表 1
    1. 有序列表 1.1
2. 有序列表 2
3. 有序列表 3
    1. 有序列表 3.1
    2. 有序列表 3.2


嵌套列表使用**tab**缩进 

---

## 四. 网页链接

```Markdown
[链接名称](链接地址)
<链接地址>
[Github]
[Github]: https://github.com/ (通常统一定义，放在页尾)
```

[百度一下](https://www.baidu.com/)

<https://www.baidu.com/>

[Github]
[Github]: https://github.com/

---

## 五. 引用

```Markdown
> 引用内容
```

> 引用内容1
> 引用内容2
> 引用内容3

```Markdown
> 一级引用
>> 二级引用
>>> 三级引用
```

> 一级引用
>> 二级引用
>>> 三级引用

---

## 六. 分割线

```Markdown
---
```

---

## 七. 删除线

```Markdown
~~被删除的内容~~
```

~~被删除的内容~~

---


## 八. 下划线

```Markdown
<u>下划线</u>
```

<u>下划线</u>

---

## 九. 表格

```Markdown
| var1 | var2  | var3 |
| :--- | :---: | ---: |
| 123  |  123  |  123 |
| 456  |  456  |  456 |
| 789  |  789  |  789 |
左对齐:-  右对齐-:  居中对齐:-:
```

| var1 | var2  | var3 |
| :--- | :---: | ---: |
| 123  |  123  |  123 |
| 456  |  456  |  456 |
| 789  |  789  |  789 |

---

## 十. 图片

```Markdown
![图片描述](图片地址)

```

![这是一张图片](./pic.jfif)

---

## 十一. 脚注

```Markdown
链接:[文字](链接)

脚注:[文字](脚注解释 "脚注名字")
```

链接 : [文字](链接)

脚注 : [文字](脚注解释 "脚注名字")

---

## 十二. 代码块

```cpp
#inlucde<iostream>
using namespace std;
int main(){
    cout << "HelloWorld" << endl;
    return 0;
}
```

```python
import numpy as np

a = np.array([[1,2,3],[3,4,5],[3,5,7]])
print(a+5)
```

---

## 十三. 表情符号

```Markdown
:表情符号:
:smile:
:laughing:
:+1:
:-1:
:clap:
```
:smile:
:laughing:
:+1:
:-1:
:clap:
更多的表情符号请查看<https://www.webfx.com/tools/emoji-cheat-sheet/>

---

## 十四. 任务列表

```Markdown
- [ ] 未勾选
- [x] 已勾选

- [ ] 任务一
  - [ ] 子任务1
  - [ ] 子任务2
- [x] 任务二
```

- [ ] 任务一
  - [ ] 子任务1
  - [ ] 子任务2
- [x] 任务二

---

## 十五. 锚点（书签）

```Markdown
格式: [锚点描述](#锚点名)
(锚点名建议使用字母和数字，区分英文大小写的，不能含有空格和特殊字符)
[返回顶部](#markdown-learn)
```

[返回顶部](#markdown-learn)
[十四-任务列表](#十四-任务列表)

---

## 十六. MPE插件的技巧

> Markdown Preview Enhanced，简称MPE

### 生成目录

- 直接在文件中输入`[TOC]`然后按回车键

### 引用文件 (可能不通用)

**MPE** 可以非常方便地引用外部文件，支持引用`.md .csv .jpg .png .gif .html .pdf`等格式的文件，引用格式: `@import "文件名"`

```Markdown
@import "gitManual.md" //.md文件的内容会被直接引用
@import "avatar.jpg" {width='200px' height='200px' title='avatar} //图片可以设置大小
@import "student.csv" //csv文件会被解析成表格
```

@import "avatar.jpg" {width='200px' height='200px' title='avatar}

@import "student.csv"

---

## 十七. MAO插件的技巧

> Markdown All in One，简称MAO

### 格式化表格

快捷键为 Alt + Shift + F

### 图片路径自动联想

---

## 十八. Paste Image插件

> 使用 Paste Image 这个插件能够直接从剪切板粘贴图片到Markdown文件中

方法1：调出命令行面板，输入`[Paste Image]`，按回车键后，截图就被插入到文件中了

方法2：使用快捷键 `Ctrl+Alt+V` (Windows系统)

粘贴的图片会被保存到当前编辑的文件所在的文件夹中，格式为PNG，并以当前时间命名。












