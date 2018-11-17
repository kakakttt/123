## 视频教程

附上我朋友录制的介绍视频链接

[https://www.bilibili.com/video/av31396414/](https://www.bilibili.com/video/av31396414/)


**但是更详细的功能还请看本文档。**
## 文字教程

有两种可供选择的模式。

- 主模式
- 专注模式

**您可以通过任务栏图标菜单切换模式。**

**全局热键**: `Shift+F1`，你可以用它来最小化和恢复`CopyTranslator`。(注：可能与部分笔记本电脑快捷键冲突)

**全局热键**: `Shift+F2`，你可以用它在`主模式`和`专注模式`中切换。

![taskbar0](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/focus_mode.png)

#### 主模式

主模式提供了一个交互式框架,可以快速地设置。

- `Stay on top`：让`CopyTranslator`窗口总是在其他窗口上方。

- `Listen on Clipboard`：监听剪贴板并自动翻译。

- `Auto copy`：如果您想在自动翻译后自动复制结果，请勾选它。

- `Smart Dict`: 启用智能词典，单词少于3的**外语句子**将被视为短语或单词，您将在专注模式上看到更详细的解释。

- `Incremental Copy`, 启用连续复制模式，将复制的文本附加到原文而不是替换它，**当段落在不同页面中分隔时尤其有用。**

- `Detect language`：自动检测源文本语言。

- `Source language`：默认是English。

- `Target language`：默认是简体中文. 

  `v0.0.6.0`后，`source`和`target`均是相对而言的，`CopyTranslator`会自动识别所复制的文字，**根据所设置的**`source`和`target`**进行自动智能互译**，也就是说，如果您复制的是`source`，会翻译为`target`，复制`target`则会翻译为`source`。（不用担心，`Auto Copy`不会与此机制相互影响。）

- `Switch Mode`: 在主模式和专注模式间切换

  ![win10.png](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/screenshot.png)
#### 专注模式

专注模式只提供一个结果窗口，让您更好地关注结果。 （注意选中`Listen on Clipboard`和`Stay on top`选项。）

1. 你可以对它自由拉伸。

   拖动窗口顶部橙色(你的电脑的主题颜色)区域,或者是边框可以拉伸变形这个窗口；

   定义**顶部蓝线以上，橙色以下偏灰色区域**为`闪区`
   - 拖动`闪区`可以整体移动窗口

   - 双击`闪区`可以隐藏窗口

   - 右击`闪区`可以复制翻译结果
     ![1528470182001](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/newfocus.png)

2. **字体可调整大小**，使用`shift + F3`和`shift + F4`缩小或增大专注模式的字体大小

   ![iMaKpT.png](https://s1.ax1x.com/2018/09/26/iMaKpT.png)
