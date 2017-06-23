## 1.SwipeRefreshLayout 的使用  ##
https://github.com/hanks-zyh/SwipeRefreshLayout
/sdcard/myfile/git.doc


## 2.Android执行打开文件(PDF,WORD,EXCEL,CHM,HTML,TEXT,AUDIO,VIDEO)的总结 ## 
http://www.cnblogs.com/loulijun/archive/2012/04/15/2450866.html
http://home.bdqn.cn/thread-57867-1-1.html

## 3.相册图片的选择   ##
https://github.com/LuckSiege/PictureSelector
https://github.com/fishwjy/MultiType-FilePicker

## 4 我的反馈界面的tab ##  
https://github.com/H07000223/FlycoTabLayout/

## 5.edittext属性设置 ##


        <EditText
            android:id="@+id/ed_search"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:textColor="@color/color_black"
            android:background="@null"  //去掉背景
            android:textCursorDrawable="@drawable/shape_edittext_cursor"  //替换光标颜色
            android:textSize="@dimen/text_design_16px" />

**控制光标显示隐藏**  http://blog.csdn.net/dongzibin/article/details/8768833    mEditSearch.setCursorVisible(false);

 **edittext设置imeOptions属性无效的解决方案**  http://blog.csdn.net/lastdream/article/details/24365633 


## 6.软键盘弹出隐藏的监听   ##
https://www.diycode.cc/topics/383

## 7. 动态修改shape 中的solid颜色 ##  
 http://yifeiyuan.me/2015/08/18/%E5%8A%A8%E6%80%81%E4%BF%AE%E6%94%B9Shape%E7%9A%84%E8%83%8C%E6%99%AF%E9%A2%9C%E8%89%B2/  

## 8.动态设置文字大小 ##
  textView.setTextSize(TypedValue.COMPLEX_UNIT_PX,getResources().getDimensionPixelSize(R.dimen.text_design_14px));  http://www.2cto.com/kf/201211/170733.html

## 9.  fragment的数据发生变化 ##
   http://blog.csdn.net/henry121212/article/details/23496913

## 10.stateLayout 包含加载load empty netError   ##
  https://github.com/gturedi/StatefulLayout
  http://www.jianshu.com/p/d727963e90b8

## 11.webview 创建销毁 ##
 http://lipeng1667.github.io/2016/08/06/memory-optimisation-for-webview-in-android/
https://github.com/zxp0505/MyWebview  //自己封装的webview


## 12.textview字体高亮显示 ##
  http://blog.csdn.net/top_code/article/details/17790363



## 13.okhttp  response.body.string为空 是因为二次查看了 ##
 http://stackoverflow.com/questions/35649829/return-response-body-string-is-empty-with-okhttp3  

## 14 动态从资源文件中获取dp大小 ##
getDimension()、getDimensionPixelSize()和getDimensionPixelOffset()的区别
 http://www.jianshu.com/p/282032797637   

## 15 progressbar  背景自定义 ##
http://blog.csdn.net/wangjinyu501/article/details/25963993

## 16. recycleview添加分割线 ##
 http://www.jianshu.com/p/4eff036360da  或者添加间隔距离项目 SpaceItemDecoration  GridLayoutManager内部设置间距 求解
## 17 .七牛上传图片0.95 ## 
 http://blog.csdn.net/guoer9973/article/details/45916709
## 18.fiddler抓包工具 ##
 http://blog.csdn.net/albert528108/article/details/21745167
## 19.scrollview内部设置math_parent不起作用 ##

 http://www.yjs001.cn/view/40579286412238472432.html

## 20. viewpager内部刷新 pageradapter.notify的时候出现的各种问题 以及fragment的使用方式  重点！！！！ ##
  http://www.jianshu.com/p/266861496508

## 21 app中全局设置字体库 ##
  https://my.oschina.net/redhouse/blog/422759?fromerr=p1JN7xix  
	https://github.com/chrisjenx/Calligraphy

## 22.scrollview滚动监听  ##
https://github.com/jzj1993/ObservableScrollView/blob/master/library/src/main/java/com/jzj/view/ObservableScrollView.java

## 23.webview加载支付宝二维码url的时候显示一下 1s跳转页面找不到的bug  ##

 			wb.setWebViewClient(new WebViewClient() {
            @Override
            public void onPageStarted(WebView view, String url, Bitmap favicon) {
                super.onPageStarted(view, url, favicon);
            }

            @Override
            public void onPageFinished(WebView view, String url) {
                super.onPageFinished(view, url);
            }

            @Override
            public boolean shouldOverrideUrlLoading(WebView view, String url) {
                String IsTrue = url.substring(0, 7);
                if (!"alipays".equals(IsTrue)) {
                    view.loadUrl(url);
                }
                return true;
            }

        });

## 24.网络状态的判断  ## 
http://www.jianshu.com/p/6e2bc3e58f88

25.将button放在相对布局里面 就没有背后的阴影了

## 26.多群岛打包  ##
http://blog.csdn.net/yy1300326388/article/details/48344411  

## 27出现找不到网页 ##
  http://blog.csdn.net/guchuanhang/article/details/52513206

## 28： 针对igore文件 ## 
		*.iml
		.gradle
		/local.properties
		/.idea/workspace.xml
		/.idea/libraries
		.DS_Store
		/build
		/captures
		.externalNativeBuild
		.idea
		*.apk

如果提交了一些本地编译的文件 需要做的是 将本地文件进行删除 提交push到git上  将git上的文件也删除了 然后再gitignore里面添加忽略文件  push到git上 最后重新编译 就好了（记得保存副本）

## 29. 侧拉删除 ##  
http://www.jianshu.com/p/9bfed6e127cc
http://blog.csdn.net/yanzhenjie1003/article/details/52115566

## 30.联系人列表： ##
 https://github.com/18722527635/MyRecyclerView  仿照这个项目里面的联系人列表进行修改 

正式版注意事项：： 1.log屏蔽 2错误信息关掉  3 swith开关关掉

## 31.沉浸式状态栏  ##
http://jaeger.itscoder.com/android/2016/02/15/status-bar-demo.html   http://www.cnblogs.com/leon-hm/p/5131323.html  https://github.com/gyf-dev/ImmersionBar

## 32.开发百度地图在6.0以上的机型定位不准 ##
 是因为so类型不够 只选了  arm64-v8a  armeabi 的全部添加 参考博客 http://blog.csdn.net/u012382791/article/details/53856203 包含位置标注  http://blog.csdn.net/qingmulang/article/details/51436855

## 33 百度地图MapView在ScrollView中的拖动黑影 ##
 http://blog.5ibc.net/p/107610.html 是因为百度地图 是opengl底层 在滑动的时候进行重绘导致的 解决方法： 1 ；将地图下载成bitmap加载到imageview中   2：百度不建议将mapview加载到scrollview

中  http://blog.csdn.net/u012565107/article/details/22067433 2；
## 34.在使用recycleview notifyItemRemoved 动态删除单个item的时候 下标错乱 ##
http://blog.csdn.net/dodouaj/article/details/51017003   

## 35 调起系统的文件管理 ## 
http://www.xjtudll.cn/Exp/428/

## 36.android 获取uuid ## 
http://blog.csdn.net/langzi7758521/article/details/52575724

37.针对写邮件中的组织架构的内存进行分析  

38 .通过intent传递大数据的时候出现 FAILED BINDER TRANSACTION !!!  (parcel size = 1327232) 是因为超出了 bind缓冲区 解决办法：（单例缓存的别的地方 持久缓存） http://blog.csdn.net/rflyee/article/details/47441405

39.  启动页面的正确姿势 解决启动白屏的问题 也和install run 有关 
自己做了很多操做  比如关闭activity默认动画(其实和这个没有关系) 后来才找到 是因为启动页 继承baseactivity  base里面也做了setcontentview操作  修改extends  AppCompatActivity 并且将延迟2s的操作放在oncreate中  就ok了
参考： 1.http://wuxiaolong.me/2017/03/13/appStart/  
	2.http://www.jianshu.com/p/cd6ef8d3d74d  

40. http://blog.csdn.net/zuiwuyuan/article/details/47904003   https://github.com/yangfuhai/ASimpleCache  数据缓存

## 41.在收件详情页面的时候 对webview进行屏幕适配 ## 
 http://www.cnblogs.com/jww-love-study/p/5194473.html  http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2013/1010/1569.cgan88/p/3361383.html

http://www.cnblogs.com/lyricgan88/p/3361383.html //针对webview。loadDataWithBaseURL 加载出文字比较小 可通过设置内部文字的大小 使其显示正常getSettings().setTextZoom(size)

## 42.scrollview内部嵌套 recycleview 当recycleview 占位不多的时候 但是内容比较多 会出现不能全部沾满的情况 添加这个属性 多一层布局 ##

android:descendantFocusability="blocksDescendants"  优先获得焦点  参考：http://www.jianshu.com/p/3815d36fd371

## 43.动态权限 ##
http://www.jianshu.com/p/c17fe97c8924  
https://github.com/googlesamples/easypermissions  //google官方的库


44.https://github.com/huzenan/EasyTransition  转场动画 打算在联系人界面和联系人详情界面做转场动画 但是联系人详情界面还有网路请求 导致的效果不佳 所以弃用

## 45.测试中发现魅族手机 选择文件 不能获取到真实的path  ##
http://blog.csdn.net/zhq217217/article/details/52767035

## 46.点击notifytion没反应 ##
http://blog.csdn.net/xy _nyle/article/details/19853591  发现4.4手机点击notifytion没反应 是因为 PendingIntent pendingIntent = PendingIntent.getActivity(appContext, notifyID, msgIntent, PendingIntent.FLAG_UPDATE_CURRENT);  里面的notifyid与环信demo的id重复 导致的 没反应  需要独一无二的

## 47.加载组织架构的时候 层级树 ##

https://github.com/shineM/TreeView

## 48.点击notify跳转到固定的activity##

 思路参考：http://www.jianshu.com/p/224e2479da18 要区分应用是否在前台 具体情况

## 49.在发布前几版出现 登陆后 会再次登陆的问题 ##
是因为序列化modle的时候没有加序列化id导致的
自动生成序列化id 参考：
在eclipse中很容易的就能自动提示添加serialVersionUID，而在AndroidStudio中却没有提示，原来是as的检查配置中默认是关掉对serialVersionUID的检查的，那么我们打开就可以。
as->preferences->Inspections->serialization issues->Serializable class without 'serialVersionUID' 勾上确认就可以