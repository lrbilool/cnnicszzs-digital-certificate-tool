# lrbilool
软件功能：
1、删除：删除根证书（序号：49:33:00:01），系统联网且未开启“关闭自动根证书更新”的情况下，根证书会自动恢复；

2、禁用：保留根证书，但置证书签发用途失效；

3、吊销：系统中吊销根证书，对于代码签名效果较好，SSL效果稍次，此时可换用“禁用”模式；

4、恢复：恢复根证书；

5、1.1版新增“关闭自动根证书更新”功能（开启本功能后，将确保上述“吊销”功能100%效果，不再因自动更新等原因，致已吊销的证书继续有效；同理，开启本功能并执行“删除”后，系统将不再自动添加CNNIC ROOT为受信任根证书）。

相关信息：
Chrome、火狐浏览器宣布删除CNNIC数字证书

谷歌4月1日更新了安全博客，宣布旗下产品将删除中国互联网信息中心（CNNIC）数字证书。而Firefox（火狐浏览器）也发布了类似声明。

Google与火狐先后发表声明称，它们旗下的浏览器，将停止信任来自中国互联网络信息中心(CNNIC)颁发的数字证书。而中国互联网信息中心(CNNIC)目前是中国最大的数字证书颁发机构。

Google表示，为缩小因此项决议受到影响的客户范围，将在限定时间内把CNNIC现有证书拉入白名单保持继续信任，而CNNIC在实现证书透明度和改进流程防止未来再次发生类似事故后可以提出撤销这一决定的申请。

此外，火狐也发表了CNNIC重新申请其授权许可的声明。火狐表示，如果CNNIC满足了Google和火狐提出的要求，这些限制将会被取消。

这也就意味着中国用户日后如果用chrome上网会带来很多不便。

也就是说，用户如果运行CNNIC根证书授权的网页，会收到安全警告的通知，比如需要重新输入登录信息；如果没有谷歌认可的根证书，一些网上银行或涉及交易资金的网页也将无法正常运行。
