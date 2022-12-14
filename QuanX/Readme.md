
# Qx断网献祭


## 添加规则

1. 将以下内容添加到 Qx 分流规则订阅，并勾选“插入资源”但是不要启用订阅规则
```
https://github.com/tom-snow/Sky_cn_xianji/raw/master/QuanX/blockAll.conf
```


2. 将以下内容添加到 Qx 分流规则订阅，并勾选“插入资源”(可以启用订阅规则)
```
https://github.com/tom-snow/Sky_cn_xianji/raw/master/QuanX/allowUserCenter.conf
```

PS: 如果你直接编辑配置文件，可以直接复制下面一段到 `[filter_remote]`
```
https://github.com/tom-snow/Sky_cn_xianji/raw/master/QuanX/allowUserCenter.conf, tag=允许光遇用户中心, update-interval=172800, opt-parser=false, inserted-resource=true, enabled=true
https://github.com/tom-snow/Sky_cn_xianji/raw/master/QuanX/blockAll.conf, tag=阻止所有请求, update-interval=172800, opt-parser=false, inserted-resource=true, enabled=false
```

## 献祭时使用

#### 无伤献祭 15.75 红蜡烛

1. 正常进入献祭图(交公粮的图)
2. 献祭两个石像
3. 进入 Qx 启用 `blockAll` 的规则(确保 `allowUserCenter` 启用着，不然可能没法进入切号界面)
4. 再次献祭几个石像，应该就会弹重连了
5. 点击切换账号再次登陆即可，(进入登陆界面就可以停用 `blockAll` 的规则了)，登陆成功就可以进入小黑屋了【成功标志，登陆后变成无翼，坐神坛进小黑屋】
6. 确定进入小黑屋就可以大退游戏，然后再进游戏，点开始后 **约2秒** 再次大退游戏，再正常进游戏
7. 进去后发现坐神坛进献祭图可以发现可以献祭但是没有红石就是成功了；如果没有成功重复步骤 6 来卡出小黑屋
8. 献祭完成后返回遇境(设置栏那就有按钮)，在暴风眼门斜坡上遁地进入暴风眼图
9. 进图后可直接回遇境再坐神坛回暴风眼等翼掉光，然后重生领红蜡烛

PS: 如果想献祭 17 红蜡烛，则在 **进行第1步前** 不要拿金人长廊的金人，完成以上 **前8步** 后再从暴风眼图飞到金人长廊那继续开启断网规则 `blockAll`，顶着弹网络重试然后领完金人，进入献祭图后再点切换账号，重新登陆后就可以再多献祭几个翼，献祭完到终点应该可以领 17 红蜡烛。(建议在金人长廊拿一个翼或者掉一个翼等弹出重试再收其他翼)


## 补充说明
为确保能有更好的效果，请进入 QuanX `设置 -> 其他设置` 中进行以下配置

1. 打开兼容性增强(非必需)
2. 关闭分流匹配优化
3. 打开 DNS 劫持
4. 关闭 MPM 温和策略机制

