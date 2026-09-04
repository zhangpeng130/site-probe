# site-probe

云端定时拨测：每约 5~20 分钟探测一次站点健康接口，连续失败时通过 WxPusher 推送微信告警，恢复后报平安。

- 逻辑全部在 `.github/workflows/probe.yml`
- 推送凭据存放在仓库 Secrets（`WXPUSHER_APP_TOKEN` / `WXPUSHER_UID`），不在代码里
- 手动测试：Actions 页面对 probe 工作流点 "Run workflow"
