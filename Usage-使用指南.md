## 视频教程

附上我朋友录制的介绍视频链接

- [Copytranslator 复译 高容错率实时翻译软件](https://www.bilibili.com/video/av31396414/) by 简约生活干货铺

最新介绍视频 2018.12.06：
- [【超强】CopyTranslator！最适合科研工作者的翻译工具](https://www.bilibili.com/video/av37503818/) by 哼哈未来

**更详细的功能还请看文字教程，CopyTranslator经过多次迭代，功能越来越丰富（~~复杂~~），不阅读完整使用指南无法完全发挥其功能，查看使用指南能够解决您90%的疑惑。**

## 文字教程

### 特性

1. 勾选`监听剪贴板`，`CopyTranslator`会自动翻译剪贴板内容。

2. `点按复制`，为减少多次按`Ctrl+C`或者是右键复制所带来的麻烦，复译引入一个选中长按自动复制的机制，在打开监听剪贴板选项后，只需选中文字，并将鼠标悬停在选中文字上方**长按不动超过0.3s后释放鼠标（其实0.3s你基本没感觉自己长按了），也就是长按后释放，即可复制。**这可以避免我们过度移动鼠标（右键再选择复制）或者是疯狂按Ctrl+C按得很累。（在一些软件中不能用，已知可用软件：文本编辑器，浏览器中，Gahhio阅读器）

   ![](https://camo.githubusercontent.com/eda5800ebf8dcf00979bd564b7e7e3ca2dd2ef80/68747470733a2f2f73312e617831782e636f6d2f323031382f30392f31332f694569624c442e676966)

3. `智能互译`，`CopyTranslator`会自动识别所复制的文本，根据所设置的`source`和`target`进行自动智能互译，也就是说，如果您复制的是`source`，会翻译为`target`，复制`target`则会翻译为`source`。（不用担心，`Auto Copy`不会与此机制相互影响。但是如果同时还打开了`检测语言` 则`智能互译`不会生效，只会将您的原文翻译成`target`语言。详细解释见Q&A）

4. `智能词典`（基于[Youdao](https://github.com/longcw/youdao)提供的API）

   单词少于3的**外语句子**将被视为短语或单词，您将在专注模式上看到更详细的解释。勾选`Smart Dict`选项以启用它。**注：查词限于有Youdao支持的语言，但是您无需也无法手动选择语言。**

    ![iManhV.png](https://s1.ax1x.com/2018/09/26/iManhV.png)



​	   ![iMaM1U.png](https://s1.ax1x.com/2018/09/26/iMaM1U.png)

4. `设置记忆`，您的设置将自动保存在磁盘中，并在下次启动时自动重新加载。配置文件版本间变动很大，又因为如果配置文件不兼容软件将直接无法使用，影响用户体验，但处理兼容性会占用较长的时间，因此决定**不向前兼容也不向后兼容，每次更新您的旧版本/新版本配置会消失。**
5. 在任务栏图标右键菜单中可以**选择界面语言（English/简体中文）**，重启CopyTranslator生效。
6. **自动检查更新**，每次启动，CopyTranslator会在后台检测更新，如果有新版本会提示，但仍需手动下载安装更新。

### 设置/选项描述

1. `始终置顶`：让`CopyTranslator`窗口总是在其他窗口上方。

2. `监听剪贴板`：监听剪贴板并自动翻译。

3. `自动复制`：如果您想在自动翻译后自动复制结果，请勾选它。

4. `智能词典`，单词少于3的`外语句子`将被视为短语或单词，您将在专注模式上看到更详细的解释。

5. `增量复制`, 将复制的文本附加到原文而不是替换它，**当段落在不同页面中分隔时尤其有用**。**用来解决一句话被页面断成两句，一次复制不全的场景**。勾选`增量复制`选项以启用它。

6. `检测语言`：自动检测源文本语言。

7. `源语言`：默认是English。`目标语言`：默认是简体中文. 

   `v0.0.6.0`后，`源`和`目标`均是相对而言的，`CopyTranslator`会自动识别所复制的文字，**根据所设置的`源`和`目标`进行自动智能互译**，也就是说，如果您复制的是`源语言`，会翻译为`目标语言`，复制`目标语言`则会翻译为`源语言`。（不用担心，`自动复制`不会与此机制相互影响。）

8. `切换模式`: 在对照模式和专注模式间切换

9. `贴边隐藏`，选项打开后

   - 专注模式窗口贴上边（Y坐标小于0）失去焦点后会自动隐藏，可设置，另外可设置翻译后自动显示。所谓失去焦点指的是，原本焦点在专注模式，而后鼠标/键盘点击其他软件，焦点转移这一事件。

   - 当专注模式处于贴边收起时可以点击其下边缘，使其获得焦点，专注模式展开。
`对照模式`暂时不会`贴边隐藏`,也不会`自动显示`。
10. `自动显示`：勾选此选项后，当专注模式处于收起状态，且监听到剪贴板变化，专注模式将自动展开。**展开后想要收起结果框，请先点击一下结果框，后点击其他地方，如果`贴边隐藏`选项处于打开状态则结果框会收起。**

11. `复制原文`，您可以通过任务栏图标的菜单/专注模式右键菜单点击`复制原文`以在`自动复制`模式下暂时复制原文，而不是译文。

    ![1537871871793](https://s1.ax1x.com/2018/09/26/iMamt0.png)

12. `切换软件语言`，在**任务栏图标右键菜单**中可以选择界面语言（English/简体中文），重启`CopyTranslator`生效。

### 双模式具体描述

有两种可供选择的模式。

- 对照模式
- 专注模式

`您可以通过任务栏图标菜单切换模式。`

`全局热键`: `Shift+F1`，你可以用它来托盘化和恢复`CopyTranslator`。(注：可能与部分笔记本电脑快捷键冲突)

`全局热键`: `Shift+F2`，你可以用它在`对照模式`和`专注模式`中切换。

![taskbar0](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/focus_mode.png)

#### 对照模式

对照模式提供了一个交互式框架,可以快速地设置，同时可以原文和译文对照着看。v0.0.8将重点增强对照模式。原文框中`Ctrl+Enter`可以快速翻译框内内容

**对照模式的关闭即为退出程序，不是托盘化。其最小化为托盘化**

![win10.png](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/screenshot.png)

#### 专注模式

专注模式只提供一个结果窗口，让您更好地关注结果。 （通常需要配合`监听剪贴板`和`始终置顶`选项使用）

1. 你可以对它自由拉伸，任意变换。

   定义下图`顶部蓝线以上，橙色以下偏灰色区域`为`闪区`

   - 拖动窗口顶部橙色(你的电脑的主题颜色)区域,或者是边框可以拉伸变形这个窗口；

   - 拖动`闪区`可以整体移动窗口

   - 双击`闪区`可以收起窗口

   - 右击`闪区`可以快速开启和关闭`监听剪贴板`功能。

   - `闪区`颜色会指示软件状态，根据你的设置会变换颜色。提示你当前是否监听剪贴板，是否打开了`自动复制`选项等等或者现在正在请求服务器翻译等等，具体颜色自行体验。

     ![1528470182001](https://gitee.com/ylzheng/CopyTranslator/raw/master/screenshot/newfocus.png)

2. 调整专注模式字体大小，使用`shift + F3`和`shift + F4`缩小或增大专注模式的字体大小

   ![iMaKpT.png](https://s1.ax1x.com/2018/09/26/iMaKpT.png)

3. 通过`专注模式`结果框的右键菜单基本可以实现全部设置及快捷操作，无需返回`对照模式`。注意这个`清空`会连剪贴板一起清空。

   ![menu](https://s1.ax1x.com/2018/09/27/iQphkT.png)

4. 拖拽文本到专注模式框，可以直接得到翻译结果(监听剪贴板时会复制拖拽的文本，当不监听剪贴板时不复制拖拽的文本)。注意，如果你是从编辑器拖拽文本过来，编辑器里的文本是会消失的，相当于剪切，`CopyTranslator`不背这锅。

5. 当光标位于专注模式结果框中时`Ctrl+Enter`实现翻译（监听剪贴板时会复制框内文本，当不监听剪贴板时不复制框内文本），`Ctrl+B`实现百度搜索框内内容，`Ctrl+G`实现Google搜索框内内容。
