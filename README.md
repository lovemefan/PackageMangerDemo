`作者:lovemefan`
`时间:2017/10/20`
# packageManagementDemo
 功能: 利用Packagemanagement类实现简单的类似launch的桌面程序,能够显示手机中的所有应用并能打开应用
 目的: 查看所有应用的pkg(PackageName)和cls(ClassName),并将所有信息复制到剪切板.获取pkg和cls信息是为了利用Intent调用其它第三方APP.
## App效果图
App名称按字母排序
![mark](http://oskhhyaq3.bkt.clouddn.com/blog/171020/8BaEE9Fibe.png?imageslim)
## 附上本人运行APP后导出的结果
|应用|pkg |cls |
| --|--|-- |
|阿里云|com.alibaba.aliyun|com.alibaba.aliyun.biz.login.WelcomeActivity|
|爱奇艺|com.qiyi.video|com.qiyi.video.WelcomeActivity|
|百度贴吧|com.baidu.tieba|com.baidu.tieba.LogoActivity|
|百度网盘|com.baidu.netdisk|com.baidu.netdisk.ui.Navigate|
|备忘录|com.samsung.android.app.memo|com.samsung.android.app.memo.Main|
|哔哩哔哩|tv.danmaku.bili|tv.danmaku.bili.ui.splash.SplashActivity|
|车来了|com.ygkj.chelaile.standard|dev.xesam.chelaile.app.module.func.SplashActivity|
|电话|com.android.contacts|com.android.dialer.DialtactsActivity|
|电子邮件|com.samsung.android.email.provider|com.samsung.android.email.ui.activity.MessageListXL|
|盖乐世空间|com.samsung.android.voc|com.samsung.android.voc.LauncherActivity|
|高德地图|com.autonavi.minimap|com.autonavi.map.activity.SplashActivity|
|高铁管家12306火车票|com.gtgj.view|com.gtgj.view.LaunchActivity|
|黑域|me.piebridge.brevent|me.piebridge.brevent.ui.BreventActivity|
|计算器|com.sec.android.app.popupcalculator|com.sec.android.app.popupcalculator.Calculator|
|交管12123|com.tmri.app.main|com.tmri.app.ui.activity.TmriActivity|
|京东|com.jingdong.app.mall|com.jingdong.app.mall.main.MainActivity|
|联系人|com.android.contacts|com.android.contacts.activities.PeopleActivity|
|猎吧出行|com.example.liabarcarandroid|com.liabarcar.guide.SplashActivity|
|浏览器|com.sec.android.app.sbrowser|com.sec.android.app.sbrowser.SBrowserMainActivity|
|录音机|com.sec.android.app.voicenote|com.sec.android.app.voicenote.main.VNMainActivity|
|南昌航空大学|com.eteasun.nanhang|com.eteasun.nanhang.activity.WelcomeActvity|
|全民K歌|com.tencent.karaoke|com.tencent.karaoke.module.splash.ui.SplashBaseActivity|
|三星健康|com.sec.android.app.shealth|com.samsung.android.app.shealth.home.HomeMainActivity|
|三星生活助手|com.samsung.android.app.sreminder|com.samsung.android.app.sreminder.phone.cardlist.SReminderActivity|
|三星视频|com.samsung.android.onlinevideo|com.samsung.android.onlinevideo.list.activity.VideoList|
|三星音乐|com.samsung.android.app.music.chn|com.samsung.android.app.music.common.activity.MusicMainActivity|
|三星阅读|com.mci.smagazine|com.chaozh.iReader.ui.activity.WelcomeActivity|
|三星云|com.samsung.multidevicecloud|com.kanbox.wp.Main|
|扫描全能王|com.intsig.camscanner|com.intsig.camscanner.WelcomeActivity|
|扇贝单词|com.shanbay.words|com.shanbay.words.startup.SplashActivity|
|设置|com.android.settings|com.android.settings.Settings|
|时钟|com.sec.android.app.clockpackage|com.sec.android.app.clockpackage.ClockPackage|
|手机淘宝|com.taobao.taobao|com.taobao.tao.welcome.Welcome|
|手机营业厅|com.sinovatech.unicom.ui|com.sinovatech.unicom.ui.WelcomeClient|
|搜狐视频|com.sohu.sohuvideo|com.sohu.sohuvideo.FirstNavigationActivityGroup|
|腾讯动漫|com.qq.ac.android|com.qq.ac.android.view.activity.SplashActivity|
|腾讯课堂|com.tencent.edu|com.tencent.edu.module.SplashActivity|
|腾讯视频|com.tencent.qqlive|com.tencent.qqlive.ona.activity.WelcomeActivity|
|通卡宝|com.nci.tkb|com.nci.tkb.ui.SplashActivity|
|网易有道词典|com.youdao.dict|com.youdao.dict.activity.DictSplashActivity|
|网易云音乐|com.netease.cloudmusic|com.netease.cloudmusic.activity.LoadingActivity|
|微博|com.sina.weibo|com.sina.weibo.SplashActivity|
|微信|com.tencent.mm|com.tencent.mm.ui.LauncherUI|
|我的文件|com.sec.android.app.myfiles|com.sec.android.app.myfiles.common.MainActivity|
|闲鱼|com.taobao.idlefish|com.taobao.fleamarket.home.activity.InitActivity.Round|
|相册|com.sec.android.gallery3d|com.sec.android.gallery3d.app.GalleryOpaqueActivity|
|相机|com.sec.android.app.camera|com.sec.android.app.camera.Camera|
|小米VR|com.mi.dlabs.vr.hulk|com.mi.dlabs.vr.hulk.launch.HulkLaunchActivity|
|信息|com.android.mms|com.android.mms.ui.ConversationComposer|
|一键锁屏|com.yujing.lockscreen|com.yujing.lockscreen.MainActivity|
|应用商店|com.sec.android.app.samsungapps|com.sec.android.app.samsungapps.SamsungAppsMainActivity|
|影梭|com.github.shadowsocks|com.github.shadowsocks.Shadowsocks|
|优酷|com.youku.phone|com.youku.phone.ActivityWelcome|
|悦动圈|com.yuedong.sport|com.yuedong.sport.main.WelcomeActivity_|
|支付宝|com.eg.android.AlipayGphone|com.eg.android.AlipayGphone.AlipayLogin|
|知乎|com.zhihu.android|com.zhihu.android.app.ui.activity.MainActivity|
|智能管理器|com.samsung.android.sm|com.samsung.android.sm.app.dashboard.SmartManagerDashBoardActivity|
|主题商店|com.samsung.android.themestore|com.samsung.android.themestore.activity.Launcher|
|租八戒|com.rentpig.customer|com.rentpig.customer.main.WelcomeActivity|
|AChm Free|com.pchen.achmfree|com.pchen.achm.MainActivity|
|Chrome|com.android.chrome|com.google.android.apps.chrome.Main|
|ES文件浏览器|com.estrongs.android.pop|com.estrongs.android.pop.app.openscreenad.NewSplashActivity|
|Excel|com.microsoft.office.excel|com.microsoft.office.apphost.LaunchActivity|
|Github|com.seasonfif.github|com.seasonfif.github.ui.activity.SplashScreenActivity|
|IT之家|com.ruanmei.ithome|com.ruanmei.ithome.ui.MainActivity|
|netkeeper|com.xinli.netkeeper|com.xinli.netkeeper.activitys.WelcomeActivity|
|ofo共享单车|so.ofo.labofo|so.ofo.labofo.activities.EntryActivity|
|QQ|com.tencent.mobileqq|com.tencent.mobileqq.activity.SplashActivity|
|RD Client Beta|com.microsoft.rdc.android.beta|com.microsoft.rdc.ui.activities.HomeActivity|
|S 换机助手|com.sec.android.easyMover|com.sec.android.easyMover.DistributionActivity|
|S 日历|com.android.calendar|com.android.calendar.AllInOneActivity|
|S Voice|com.samsung.voiceserviceplatform|com.samsung.voiceserviceplatform.ui.SVoiceMainActivity|
|Samsung Gear|com.samsung.android.app.watchmanager|com.samsung.android.app.watchmanager.setupwizard.SetupWizardWelcomeActivity|
|Super Pads|com.opalastudios.pads|com.opalastudios.pads.ui.MainActivity|
|Survival Online|com.gameline.survivalcraftfree|com.unity3d.player.UnityPlayerActivity|
|TapTap|com.taptap|com.play.taptap.ui.MainAct|
|UC浏览器|com.UCMobile|com.UCMobile.main.UCMobile|
|USIM卡应用|com.android.stk|com.android.stk.StkLauncherActivity|
|WiFi万能钥匙|com.snda.wifilocating|com.lantern.launcher.ui.MainActivity|
|Word|com.microsoft.office.word|com.microsoft.office.apphost.LaunchActivity|