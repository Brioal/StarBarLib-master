
## 效果图:
![](https://github.com/Brioal/StarBarLib-master/blob/master/art/1.gif)
## 使用方法
### 1.在项目的build.gradle文件做如下修改
```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
### 2.在app的build.gradle内作如下修改
```
dependencies {
      ...
	    compile 'com.github.Brioal:StarBarLib-master:1.0'
      ...
}
```
## 提供的方法
 方法 | xml属性 | 作用
 --- | --- | ---
 `setTouchable(boolean touchable)` | `isTouchable` | 设置是否可以通过触摸改变星级
 `setStarFillBitmap(Bitmap starFillBitmap) ` | `starFill` | 设置满星级的图片
 `setStarEmptyDrawable(Drawable starEmptyDrawable) ` | `starEmpty` | 设置空星级的图片
 `setStarCount(int starCount) ` | `starCount` | 设置星级的总数
 ` setStarSize(int starSize)` | `starSize` | 设置星级的大小
 ` setStarDistance(int starDistance)` | `starDistance` | 设置星星之间的间距
 `setIntegerMark(boolean integerMark)` | `setIntegerMark ` | 设置是否是整数星级
 `setStarMark(float mark)` | ` ` | 设置要显示的星级
 `float getStarMark()` | ` ` | 获取显示的星级
## 使用方法
### xml布局
```
    <com.brioal.starbar.StarBarView
        android:layout_centerInParent="true"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:starCount="8"
        app:starDistance="5dp"
        app:isTouchable="true"
        app:starEmpty="@drawable/ic_star_empty"
        app:starFill="@drawable/ic_star_full"
        app:starSize="30dp"/>

```
## 完毕
