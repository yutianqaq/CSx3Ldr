> 免责声明：本工具仅供安全研究和教学目的使用，用户须自行承担因使用该工具而引起的一切法律及相关责任。作者概不对任何法律责任承担责任，且保留随时中止、修改或终止本工具的权利。使用者应当遵循当地法律法规，并理解并同意本声明的所有内容。



一个 Cobalt Stirke 插件，依赖 nim。

**注意：icon 需要在 /tmp/icon.o**

**安装 nim 环境**

```
apt isntall nim
nimble install winim
```

过 qvm 需要图标。编一个放 /tmp目录 名为 icon.o

加载后，工具会出现在 attack -> CSx3Ldr。

也可以使用快捷键 Ctrl + J。

过不了就换 icon

## 效果图

![image-20240107153547666](img/image1.png)

## 

## 换 icon

**icon.rc**

```
demo2 ICON "app.ico"
```

找小的 ico 图标，比如 5kb、10kb 的

```
> x86_64-w64-mingw32-windres -F pe-x86-64 icon.rc -O coff -o icon.o

> cp icon.o /tmp/icon.o
```





# 参考 

https://github.com/RCStep/CSSG

https://github.com/hack2fun/BypassAV/tree/master
