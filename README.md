# KLPTID-PROJECT
一个通过帖子TID、用户UID等值快速跳转对应帖子、用户空间等工具，适用于KLPBBS等Dz论坛。

## 使用方法
1. 在您的HTML文件引入此 JavaScript 代码，推荐在写在**body**中。
```html
<script src="index.js"></script> //请使用您自己的地址
```
2. 在您的HTML文件中，在**body**中写入：
```html
<script>
    const skipper = new TIDSKIPPER1();
</script>
```
这样您就有了一个十分简朴的跳转器，实现基本功能。
![图1](https://tikolu.net/i/ftxqe)
详细见“跳转器”

## 跳转器
KLPTID-PROJECT 有4个版本的跳转器，可见下表格：
|跳转器名|用途|加入版本|
|-------|-------|-------|
|TidSkipper1|直接跳转对应帖子|v1.0.0|
|TidSkipper2|选择浏览模式跳转对应帖子|v1.0.0|
|UserSkipper1|直接跳转对应用户空间|v1.0.0|
|UserSkipper2|选择浏览模式跳转对应用户空间|v1.0.0|

如果要使用其中一个，只需像使用方法2中new一个跳转器对应的类名(同名)。
> v1.0.0: 一种只能创建一个跳转器，后版本将会修复。

同时，您也可以自定义CSS来美化，下面就是一个示例：
![图2](https://tikolu.net/i/cbtfz)

## 开源协议
本项目使用MIT协议，见本仓库License。

## 累积STAR
![GitHub stars](https://img.shields.io/github/stars/klp-xkjt/KLPTID-PROJECT)
