##iOS上架app流程

1. 去[apple网站](https://developer.apple.com/account/ios/identifier/bundle/create)填写app id description,name和工程名字一样
2. 填写app bundle id `com.xxxxx.SManager`,然后选中自己的需求，如果有远程推送记得钩上。
3. 创建证书：点开mac->luanchpad->others->keyaccess,填写开发者邮箱即可
4. 回到刚才网站创建发布证书 ：点`ALL` ->`右上角 + ` ->` App Store and Ad Hoc`,然后下载 `ios_distribution.cer`
5. 在本机安装改证书，双击即可，选中system
6. 创建配置文件：在上面的网站里面选择`Provisioning Profiles`->`all`->`+`->`Distribution(App Store)`，然后点点点，选中自己最新申请的证书,name profile:`coms.xxxxx.SManager_profile`,填写一个特殊名字即可

##打包
1. 选中你的项目，选中`project->code sign`，选择 `profile...`
2. x选择xcode menu的 `Product--Archive`，连接真机打包，一路点击下去即可

最后添加几个图，用于日后回忆
