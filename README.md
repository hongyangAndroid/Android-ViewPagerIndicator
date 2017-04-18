# Android-ViewPagerIndicator
一款仿MIUI的ViewPagerIndicator，支持Tab数量随意定义。

# 效果图

## 固定tab数量
![Sample Screenshots][1]
## 非固定tab数量
![Sample Screenshots][2]

# 用法

## 代码生成tab

	mIndicator.setVisibleTabCount(4);//设置可见Tab数量
	mIndicator.setTabItemTitles(mDatas);//设置tab标题
	mViewPager.setAdapter(mAdapter);
	mIndicator.setViewPager(mViewPager,0);//绑定ViewPager

## 直接布局中书写
布局中编写，则代码中只需要绑定ViewPager一行代码。
	
	<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:zhy="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#ffffffff"
    android:orientation="vertical" >

    <com.zhy.view.ViewPagerIndicator
        android:id="@+id/id_indicator"
        android:layout_width="match_parent"
        android:layout_height="45dp"
        android:background="@drawable/title_bar_bg_one_row"
        android:orientation="horizontal"
        zhy:visible_tab_count="3" >

        <TextView
            android:layout_width="0dp"
            android:layout_height="fill_parent"
            android:layout_weight="1"
            android:gravity="center"
            android:text="短信1"
            android:textColor="#CCFFFFFF"
            android:textSize="16sp" />

        <TextView
            android:layout_width="0dp"
            android:layout_height="fill_parent"
            android:layout_weight="1"
            android:gravity="center"
            android:text="收藏2"
            android:textColor="#CCFFFFFF"
            android:textSize="16sp" />

        <TextView
            android:layout_width="0dp"
            android:layout_height="fill_parent"
            android:layout_weight="1"
            android:gravity="center"
            android:text="推荐3"
            android:textColor="#CCFFFFFF"
            android:textSize="16sp" />

        <TextView
            android:layout_width="0dp"
            android:layout_height="fill_parent"
            android:layout_weight="1"
            android:gravity="center"
            android:text="推荐4"
            android:textColor="#CCFFFFFF"
            android:textSize="16sp" />
	 </com.zhy.view.ViewPagerIndicator>

	    <android.support.v4.view.ViewPager
		android:id="@+id/id_vp"
		android:layout_width="match_parent"
		android:layout_height="0dp"
		android:layout_weight="1" >
	    </android.support.v4.view.ViewPager>

	</LinearLayout>



# 关于我

[我的博客地址][3]

[1]: https://github.com/hongyangAndroid/Android-ViewPagerIndicator/blob/master/fixed_item.gif
[2]: https://github.com/hongyangAndroid/Android-ViewPagerIndicator/blob/master/more_items.gif
[3]: http://blog.csdn.net/lmj623565791
