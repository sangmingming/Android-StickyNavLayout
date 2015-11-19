# Android-StickyNavLayout
An android library for navigator that stick on the top 



## 效果图

![](sc.gif)


## 用法
直接作为跟布局，内部一次放置，顶部内容区域，导航，底部布局。 注意，必须包含三个子布局。底部布局必须为，ViewPager，或者ListView，RecyclerView，ScrollView，或子类。

```xml
<me.isming.stickynavlayout.StickyNavLayout xmlns:tools="http://schemas.android.com/tools"
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical" >

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="300dp"
        android:background="#4400ff00" >

        <TextView
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:gravity="center"
            android:text="软件介绍"
            android:textSize="30sp"
            android:textStyle="bold" />
    </RelativeLayout>

    <com.zhy.view.SimpleViewPagerIndicator
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:background="#ffffffff" >
    </com.zhy.view.SimpleViewPagerIndicator>

    <android.support.v4.view.ViewPager
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="#44ff0000" >
    </android.support.v4.view.ViewPager>

</me.isming.stickynavlayout.StickyNavLayout>
```


## 感谢

项目来源自hongyang的代码，在其基础上修改，原代码在:[https://github.com/hongyangAndroid/Android-StickyNavLayout](https://github.com/hongyangAndroid/Android-StickyNavLayout) , 在其基础上修改一些bug，以及支持底部根布局不必必须为ViewPager，以及三个View不比指定id。

同时，感谢[@ta893115871](https://github.com/ta893115871) 修改的bug [上下滑动 列表 有时会触发OnItemClick事件 ，几率出现](https://github.com/hongyangAndroid/Android-StickyNavLayout/issues/9)


## 关于我

blog:[blog.isming.me](http://blog.isming.me)

mail: linming1007@gmail.com

weibo: [@码农明明桑](http://weibo.com/mingmingsang)