## v0.0.6.1 已知问题:
1. 自动检测语言会更改source，会导致智能互译的操作逻辑异常混乱
2. 32位的版本会出现奇怪的bug，比如经常性`网络错误`，以及`Auto Copy`失效等情况。

## v0.0.6.0 已知BUG:
1. 貌似主模式的手动translate不能用了，已在v0.0.6.1修复。平时也不怎么用手动translate，都是打开剪贴板监听。我感觉有了`增量复制`以后就基本用不着手动translate了。想不出啥场景了。

2. 好像有时候`smart dict`会莫名奇妙查询一个词`ENG`,但是不影响使用。

## 问答
1. 智能互译在打开自动检测语言时失效？

    答：复制英文翻译成中文，复制中文翻译成英文，更新日志第一条，其他语言设置下source和target就可以，**我一般不开自动检测语言的**，你想想看，如果自动检测语言检测到原文是中文，然后你设置的target也是中文，我总不至于给你翻译成英文吧？**只有说不开自动检测语言，他才会`智能互译`**。如果你开了检测语言，source就无效了，那我肯定只能给你翻译成target。如果没开检测语言，我就认为souce和target需要互相转换。自动检测语言是用来翻译其它语言比较好用，**用来翻译不知道是啥语言的**

2. 增量复制的应用场景？

    答： 增量复制是用来解决一句话被页面断成两句，一次复制不全的场景

3. 这个翻译框如果ctrl+A能全选就好了？

    答： 你翻译框想要ctrl+a是要复制啥？右键菜单里都有，专注模式的结果框的右键菜单里基本啥都有了，我感觉都不太需要回到主模式，`clear`, `copy result`, `copy source`,不过这个`clear`会连剪贴板一起清空

4. 点按翻译不好用？

    答：他只是模拟ctrl+c而已，至于能不能复制到不知道了。**不是点一下，是按0.3s,你得先选中，然后移动到选中文字上方，按0.3s放开**。我觉得挺好用的其实，如果ctrl+c的话，其实鼠标键盘切换很累的，这个就直接鼠标就可以，而且还不用右键菜单费神找复制选项。这是不知道划译怎么做的凑合方案。你按太久也没啥意义，**我检测的是你的鼠标释放的瞬间，跟你按下的时间间隔，以及鼠标的偏移量不太大就会模拟一次ctrl+c**。**但是我知道abobe的阅读器就不能用**，我用的gaahio就很舒适，**有些阅读器刚按一下，没放开就取消选中了，那我这个模拟ctrl+c肯定没办法的。**另外，有一大堆广告的恶心人的foxit也不建议使用，谁用谁知道，任务栏莫名其妙的广告，闪来闪去。