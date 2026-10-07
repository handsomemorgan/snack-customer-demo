# 取餐有约 · 顾客手机演示

[手机在线体验](https://handsomemorgan.github.io/snack-customer-demo/)

这是单独的顾客手机点单案例，不显示店家或超管导航。选择左侧分类、添加餐品、滑动预约时间并提交，查看模拟票据。团建入口直接展示店家联系方式。

## 演示边界

不进行真实交易，无支付宝支付、真实打印机或营业后端。请勿输入真实个人资料。数据在访问者自己的浏览器保存；不同设备不共享。示例电话0571-0000-0000不可拨号。店家示例不是销售收入。

两个演示仓库在同一个 GitHub 域名下，在同一浏览器使用同一份模拟店铺数据：店家修改可以影响该浏览器中的顾客演示，顾客模拟预约也能出现在店家演示。不同手机或浏览器互不共享；浏览器禁用持久存储时功能可能受限。

## 打开另一个演示

[顾客点单](https://handsomemorgan.github.io/snack-customer-demo/) · [店家工作台](https://handsomemorgan.github.io/snack-merchant-demo/) · [完整多租户Demo](https://handsomemorgan.github.io/snack-pickup-demo/)

## 本地预览与更新

Node.js >=22.13：

```sh
npm ci
npm run build:pages
npm run preview:pages
```

这个仓库的构建配置已设置为 customer 版，路径为 /snack-customer-demo/。GitHub Pages 从 main 分支 /docs 发布。修改后重新构建并提交 docs；不要上传 .env.local、.dev.vars、数据库、实际商户密钥或报名材料。

44项浏览器模拟与30项本地接口检查已通过；实际手机浏览器操作另行验证滚轮、侧栏、弹窗与320/390/430像素屏幕宽度。自动检查不证明真实支付或硬件可用。

## 来源

共享取餐有约源码。React、Vinext、Drizzle与已有shadcn组件；vendor和build中的原始许可保留。AI示意餐品图不是商家实拍。本地后端开发见LOCAL_DEVELOPMENT.md。GitHub Pages只承担功能演示，[使用限制](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)。
