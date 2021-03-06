#CircleTextView(圆形+文字View)
基于
[CircleTextImageView](https://github.com/CoolThink/CircleTextImageView),
[CircleImageView](https://github.com/hdodenhof/CircleImageView)开源库修改


1.只显示头像
2.圆形背景文字
3.头像+文字
![头像+文字](https://github.com/mysiga/CircleTextView/blob/master/CircleTextView.jpeg)

使用方法:

###只显示头像
```
<com.mysiga.lib.view.CircleTextView
            android:id="@+id/profile_image"
            android:layout_width="96dp"
            android:layout_height="96dp"
            android:src="@drawable/hugh"
            app:borderColor="#FF000000"
            app:borderWidth="2dp" />
```
###纯色圆形背景+文字

```
<com.mysiga.lib.view.CircleTextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:text="照片"
            android:textColor="@android:color/white"
            android:textSize="32sp"
            app:backgroundColor="@color/colorAccent"
            app:borderColor="@android:color/white"
            app:borderWidth="2dp"
            app:textPadding="35dp" />
```
###头像+文字

```
<com.mysiga.lib.view.CircleTextView
            android:layout_width="96dp"
            android:layout_height="96dp"
            android:layout_gravity="center"
            android:src="@drawable/skye"
            android:text="晴朗"
            android:textColor="#ff99cc00"
            android:textSize="32sp"
            app:backgroundColor="#50555D"
            app:borderColor="@android:color/darker_gray"
            app:borderWidth="2dp"
            app:textPadding="35dp" />
```
引入设置

```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
```
implementation 'com.github.mysiga:CircleTextView:V1.1'
```
混淆编译配置
```
-keep class android.support.v7.widget.** { *; }
```
