# 代码比较报告

核对日期：2026-10-02（Asia/Shanghai）。

## 来源

- 本地原文件：`[银河奶牛]康康运气_修复.txt`，头部版本 `0.2.2`。
- 线上来源：[Greasy Fork 546427 当前安装脚本](https://greasyfork.org/zh-CN/scripts/546427)，版本 `0.2.4`。
- 本地原文件：293431 字节，6344 行。
- 下载的线上文件：293763 字节，6346 行。

## 结果

完整文件比较只发现三个元信息字段的差异：

| 字段 | 本地 | 线上 |
| --- | --- | --- |
| `@version` | `0.2.2` | `0.2.4` |
| `@downloadURL` | 无 | Greasy Fork 添加的安装文件地址 |
| `@updateURL` | 无 | Greasy Fork 添加的版本检查地址 |

其他所有代码、注释和元信息字段逐字一致。对文件文本按行标准化换行，并删除上述三个元信息字段后，两者 SHA-256 均为：

```text
55b894f9550acea79c09d04ffd118e1da9623fd39fc9ae1b608d793df5e9f94f
```

因此本地代码没有缺少线上功能；版本号差异不能作为功能新旧的依据。本仓库以相同代码的 `0.2.4` 作为初始版本。

## 本次整理

原文件移动为 `kangkang-luck.user.js`，唯一代码修改是将 `@version` 从 `0.2.2` 校正为 `0.2.4`。未复制 Greasy Fork 自动添加的更新地址；从 Greasy Fork 安装时由其生成。`@name`、`@namespace`、作者、许可证和脚本正文保持原样。

验证范围为完整文本比较和 JavaScript 语法检查，不包括游戏中的运行回归测试。本次没有修改脚本运行逻辑。

## 原始差异

```diff
--- local-0.2.2
+++ greasyfork-0.2.4
@@ -1,7 +1,7 @@
 // ==UserScript==
 // @name         [银河奶牛]康康运气_修复
 // @namespace    http://tampermonkey.net/
-// @version      0.2.2
+// @version      0.2.4
 // @description  更详细的统计数据（建议搭配 MWITools 获得中文物品名）
 // @author       Weierstras@www.milkywayidle.com
 // @license      MIT
@@ -16,6 +16,8 @@
 // @require      https://cdn.jsdelivr.net/npm/chart.js@4.4.3/dist/chart.umd.min.js
 // @require      https://cdn.jsdelivr.net/npm/ml-fft@1.3.5/dist/ml-fft.min.js
 // @require      https://cdn.jsdelivr.net/npm/lz-string@1.5.0/libs/lz-string.min.js
+// @downloadURL https://update.greasyfork.org/scripts/546427/%5B%E9%93%B6%E6%B2%B3%E5%A5%B6%E7%89%9B%5D%E5%BA%B7%E5%BA%B7%E8%BF%90%E6%B0%94_%E4%BF%AE%E5%A4%8D.user.js
+// @updateURL https://update.greasyfork.org/scripts/546427/%5B%E9%93%B6%E6%B2%B3%E5%A5%B6%E7%89%9B%5D%E5%BA%B7%E5%BA%B7%E8%BF%90%E6%B0%94_%E4%BF%AE%E5%A4%8D.meta.js
 // ==/UserScript==
 
 
```
