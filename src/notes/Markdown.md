
---

## 📝 一、基础语法

### 1. 标题

markdown

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

### 2. 段落与换行

```markdown
这是一个普通段落。

这是第二行，注意前面没有空格。
```

### 3. 强调与删除线
```markdown
**加粗文本**
*斜体文本*
***加粗斜体文本***
~~删除线文本~~
```
**加粗文本**
*斜体文本*
***加粗斜体文本***
~~删除线文本~~

### 4. 列表

#### 无序列表

```markdown
- 项目1
- 项目2
  - 子项目1
  - 子项目2
```
- 项目1
- 项目2
  - 子项目1
  - 子项目2
#### 有序列表
```markdown
1. 第一项
2. 第二项
3. 第三项
```
1. 第一项
2. 第二项
3. 第三项
### 5. 链接与图片
```markdown
[链接文本](https://example.com)
![替代文本](https://example.com/image.jpg)
```
[链接文本](https://example.com)
![替代文本](https://example.com/image.jpg)
### 6. 分隔符
```markdown
---
```

---
```markdown
## 📌 二、代码与数学公式

### 1. 代码块



````
```python
def hello():
    print("Hello, Markdown!")
````


### 2. 内联代码
```markdown
这是内联代码：`print("Hello")`
````

````

### 2. 内联代码
```markdown
这是内联代码：`print("Hello")`
````

### 3. 数学公式（LaTeX）


```markdown
$$
E = mc^2
$$
```

---

## 📁 三、表格



```markdown
| 列1 | 列2 | 列3 |
|-----|-----|-----|
| 数据1 | 数据2 | 数据3 |
| 数据4 | 数据5 | 数据6 |
```

| 列1 | 列2 | 列3 |
|-----|-----|-----|
| 数据1 | 数据2 | 数据3 |

---

## 📄 四、引用与块引用
```markdown
> 这是一个块引用。
> 它可以跨越多行。

这是普通段落。
```

> 这是一个块引用。
> 它可以跨越多行。

这是普通段落。

---

## 📈 五、其他功能

### 1. 转义字符
```markdown
\*星号\* 会被转义为 *星号*
```

\*星号\* 会被转义为 *星号*

### 2. 自定义标题ID


```markdown
## 标题 {#custom-id}
```

## 标题 {#custom-id}

### 3. 任务列表
```markdown
- [ ] 未完成的任务
- [x] 已完成的任务
```
- [ ] 未完成的任务
- [x] 已完成的任务

---

## 🧠 六、高级技巧

### 1. 语法高亮（需配合代码块）


````markdown
```python
for i in range(10):
    print(i)
````

```python
for i in range(10):
    print(i)
```
### 2. 多语言支持
````markdown
```javascript
console.log("Hello, Markdown!");
````

```javascript
console.log("Hello, Markdown!");
````

### 3. 自动链接
````markdown
```
[https://example.com](https://example.com)
```


```markdown
[https://example.com](https://example.com)
````

---

## 📌 常见问题

|问题|解决方案|
|---|---|
|为什么代码块没有高亮？|确保使用支持语法高亮的编辑器（如 VS Code、Typora）|
|如何添加图片？|使用 `![替代文本](图片链接)` 格式|
|如何让列表项缩进？|在列表项前添加空格（如 `- 子项`）|

---

## 📚 参考文档

- [Markdown 官方语法指南](https://commonmark.org/)
- [GitHub Flavoured Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-API-Specification)

---

