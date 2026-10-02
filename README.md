# [银河奶牛]康康运气_修复

银河奶牛放置的统计脚本。当前版本：`0.2.4`。

- 安装与反馈：[Greasy Fork 546427](https://greasyfork.org/zh-CN/scripts/546427)
- 唯一维护文件：`kangkang-luck.user.js`
- 原作者：脚本元信息中的 `Weierstras@www.milkywayidle.com`，原始脚本与参考项目见代码中的署名和链接。
- 许可：MIT（沿用脚本原有 `@license` 声明）。

## Greasy Fork 同步配置

在现有脚本 546427 的管理页面配置代码同步，来源地址为：

```text
https://raw.githubusercontent.com/Yinhaoran1128/niuniu-userscripts/main/kangkang-luck.user.js
```

然后登录 [Greasy Fork Webhook 配置说明](https://greasyfork.org/zh-CN/users/webhook-info)，取得 Payload URL 和 Secret。在本仓库 `Settings → Webhooks → Add webhook` 中按该页面说明填写，Content type 使用 `application/json`，事件选择 `Just the push event`，保持 Active 启用。

本仓库建立时尚未配置 Greasy Fork 同步或 Webhook；仓库推送不会自动改变现有 Greasy Fork 发布内容。

官方说明：[API 与 Webhook](https://greasyfork.org/zh-CN/help/api)。

## 以后更新

进入这个独立仓库目录操作：

```sh
cd kangkang-luck
```

1. 修改 `kangkang-luck.user.js`，在游戏中验证。
2. 正式发布时递增头部 `@version`，保持 `@name` 和 `@namespace`。
3. 检查语法并查看差异：

```sh
node --check kangkang-luck.user.js
git diff
```

4. 提交和推送：

```sh
git add kangkang-luck.user.js
git commit -m "release: 更新版本与说明"
git push origin main
```

5. 接入 Webhook 后，检查 GitHub 的 Recent Deliveries 和 Greasy Fork 的版本、同步状态。

开发中的改动放在其他分支；`main` 保存准备发布的版本。需要单独控制发布时机时，可在后续改用 Release 事件和 Release 附件同步。

## 初始版本核对

2026-10-02 完整比较本地脚本与 Greasy Fork 当前安装文件：忽略 `@version` 和 Greasy Fork 添加的 `@downloadURL`、`@updateURL` 后，代码逐字一致。仓库初始版本采用 `0.2.4`，没有修改运行逻辑。

详情见 [比较报告](docs/code-comparison.md)。
