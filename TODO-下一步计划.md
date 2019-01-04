## Phoenix 计划
之后版本的CopyTranslator界面不再使用wxpython编写，而使用Electron实现，这并不意味着CopyTranslator将会是纯Node实现，而是会是一种混合语言的实现，前端使用Electron+Vue展现精美的界面，后端是python编写的微型服务器，提供node当前暂时不支持的系统级操作，比如模拟键盘输入，监听鼠标事件等等，前后端通过TCP/IP协议交互。这是一种全新的思路，能够让我们同时发挥两种动态语言的优势，快速构建原型，快速迭代。

问：为什么后端仍然使用python实现，而不是纯node？

答：我也想纯node实现，但是因为CopyTranslator很多功能，比如模拟键盘输入，监听鼠标事件等等，以及后续可能加入的其他的功能，node并未实现，自己实现费时费力；其次，使用python做后端，可以最大程度复用之前的代码，在过渡时期，可能大多数工作都是由后端完成，在过渡完成后，大多数工作应该都会由前端完成。至于为什么不用C或者其他的语言，不好意思，第一性能上python完全够用，第二python的现成的包多，用C开发效率不高。这是一个小工具，我觉得开发效率比程序执行的效率要重要得多。

问：新的版本和当前版本会有什么不同呢？

答：
1. 界面更漂亮，1是因为使用的Electron+Vue有大量漂亮的可复用UI组件，2是设计师[Mārtiņš Zemlickis](http://mzemlickis.lv/)将为CopyTranslator重新设计界面，交互逻辑。
2. 体积变大，现在估计压缩包的体积会是40~50M左右，因为装了一个chromium和python环境，想不大都不太可能吧。。。。。
3. 代码更优雅，前后端分离真的是一个很棒的设计说实话。

总而言之，敬请期待吧 

Phoenix项目现在在这里开发[https://github.com/elliottzheng/CopyTranslator-Phoenix](https://github.com/elliottzheng/CopyTranslator-Phoenix)，完成后会合并到本仓库。


## v0.0.8 驺吾 
v0.0.8 神奇生物版本代号--[驺吾/Zouwu](https://baike.baidu.com/item/%E9%A9%BA%E5%90%BE)

计划详情见[Project v0.0.8 Zouwu](https://github.com/elliottzheng/CopyTranslator/projects/1)

明年见。

## 遥遥无期
- 英语语法检查，写作的时候应该还比较有用。
- ~~PDF完全解析~~ 个人感觉工作量大而且效果不好？就算能做，效果也会很差。翻译总是需要人工校对的。格式啥的也会是个大问题。

更多改进意见欢迎在Issue中提出。
