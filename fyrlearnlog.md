### Android和IOS的调研与学习

#### Android调研学习
    今天填写了需求文档，需求分析，分析了自己负责的小区服务、小区论坛、物业通知三个模块的需求。
    也下载了Android studio和Xcode，初步调研了把我们的程序转化为Android和iOS程序的难度和可行性。
——————2019/7/3

#### MongoDB建立小区论坛和论坛评价
    今天完成了MongoDB建立小区论坛和论坛评价的任务，看完了Android学习的12个视频。
    -activity七个生命周期，
        1、当第一次调用一个Activity就会执行onCreate方法
        2、当Activity处于可见状态的时候就会调用onStart方法
        3、当Activity可以得到用户焦点的时候就会调用onResume方法
        4、当Activity被遮挡住的时候就会调用onPause方法
        5、当Activity处于不可见状态的时候就会调用onStop方法
        6、当Activity没有被销毁的时候重新调用这个Activity就会调用onRestart方法
        7、当Activity被销毁时会调用onDestory方法

    -intent 用来在activity之间传递消息，activity不一定在同一个应用程序中
    -activity初步布局；有horizontal水平的和vertical垂直的两种
    
    -通过task来把不同程序或相同程序的activity组织在一起，将activity压入栈中，activity.finish()摧毁
    activity，会从栈中去掉
    -linerLayout与TableLayout的使用方法
    -常见控件有TextView,EditText,Button,Menu这几种
    -了解布局和常用控件
        · 相对布局，就是与其他部件的相对布局
        · toast 吐司，提示用户消息
        · RadioGroup和RadioButton 单选框
        · CheckBox 复选框
        · pregressbar 进度条 可自定义最大值、主进度条、第二进度条  
        · 默认进度条无法显示进行的状态
        · listView extend listActivity显示像列表一样的布局
——————2019/7/4

#### 写系统设计文档自己负责的部分

    包括小区服务，物业通知，小区论坛三个部分，要写模块功能，各个功能的类图，还要写时序图，和用到哪些类及其描述
——————2019/7/5
#### 写小区论坛

    删除帖子、删除评论，写小区论坛的测试，开始写物业通知模块。
——————2019/7/8

#### 写物业通知模块

    写小区物业通知模块，完成物业通知模块的测试。
    难点有：id自增。数据库的表noticeId在entity中对应的应该写成noticeid（不然会报找不到表的操作）。
    通过自己写的sql语句判断数据库中有没有某行。
    通过自己写的sql语句删除数据库中某行失败，只能先取出这个对象，然后用jpa自带的delete将它删除。
————————2019/7/9
