# KLPTID-PROJECT 

[![GitHub stars](https://img.shields.io/github/stars/klp-xkjt/KLPTID-PROJECT?style=for-the-badge)](https://github.com/klp-xkjt/KLPTID-PROJECT/stargazers)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

论坛快捷跳转工具，通过帖子TID和用户UID等实现快速页面跳转，适配KLPBBS等Discuz论坛系统。

## 功能特性
- 零依赖纯JavaScript实现
- 双模式跳转（直接跳转/浏览模式选择）
- 支持帖子与用户空间跳转
- 高度可定制化样式
- 跨平台兼容性

## 快速开始
### 基础集成
1. 在HTML文件的`<body>`末尾添加脚本引用：
```html
<script src="path/to/KLPTID.js"></script>
```

2. 初始化跳转控制器：
```html
<script>
  // 选择需要的跳转器类型（四选一）
  const skipper = new TIDSKIPPER1(); // 帖子直接跳转
  // const skipper = new TIDSKIPPER2(); // 帖子浏览模式跳转
  // const skipper = new USERSKIPPER1(); // 用户空间直接跳转
  // const skipper = new USERSKIPPER2(); // 用户空间浏览模式跳转
</script>
```

### 效果预览
![跳转器界面示例](https://tikolu.net/i/ftxqe)  
*基础跳转器界面*

![自定义样式示例](https://tikolu.net/i/cbtfz)  
[体验DEMO](https://klp-xkjt.github.io/KLPTIDJS/) | [样式源码](https://github.com/klp-xkjt/klp-xkjt.github.io/blob/main/KLPTIDJS/index.html)

## 所有跳转器
| 组件名称         | 功能描述                     | 跳转模式       | 引入版本 |
|------------------|----------------------------|---------------|----------|
| `TidSkipper1`    | 帖子直达跳转                | 直接跳转      | v1.0.0   |
| `TidSkipper2`    | 带浏览模式的帖子跳转        | 模式选择      | v1.0.0   |
| `UserSkipper1`   | 用户空间直达跳转            | 直接跳转      | v1.0.0   |
| `UserSkipper2`   | 带浏览模式的用户空间跳转    | 模式选择      | v1.0.0   |

## 样式定制

下面是各转换器内输入框、跳转按钮等元素的类名，可用于CSS定义：

| 跳转器名称      | 容器类 (CSS Class)   | 输入框ID (Input) | 按钮ID (Button) | 模式切换器ID (Mode Switcher) |
|-----------------|----------------------|------------------|-----------------|------------------------------|
| TIDSKIPPER1     | `tid-skipper-v1`     | `skip-input1`    | `skip-button1`  | N/A                          |
| TIDSKIPPER2     | `tid-skipper-v2`     | `skip-input2`    | `skip-button2`  | `mode-switcher2`             |
| USERSKIPPER1    | `user-skipper-v1`    | `skip-input3`    | `skip-button3`  | N/A                          |
| USERSKIPPER2    | `user-skipper-v2`    | `skip-input4`    | `skip-button4`  | `mode-switcher4`             |

```css
// 示例

```

## 协议声明
本项目采用 [MIT License](LICENSE) 开源协议，您可以自由地进行：
- 商业使用 
- 修改分发 
- 专利使用 
- 私用存储 

唯一要求：**保留原始版权声明**
