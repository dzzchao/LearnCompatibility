# [Compatibility](https://developer.android.google.cn/guide/practices/screens_support.html)
## 适配不同的语言

字符串，新增不同的 values 目录和 string.xml 文件。<br/>
例如：新增 res/values-en/string.xml。<br/>

```
// Get a string resource from your app's Resources
String hello = getResources().getString(R.string.hello_world);

// Or supply a string resource to a method that requires a string
TextView textView = new TextView(this);
textView.setText(R.string.hello_world);
```


```
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="@string/hello_world" />
```

## 适配不同的屏幕
- 尺寸：按屏幕对角测量的实际物理尺寸。
- 屏幕密度：屏幕物理区域中的像素量；通常称为 dpi（每英寸 点数）。
- 方向：从用户视角看屏幕的方向，即横屏还是 竖屏，分别表示屏幕的纵横比是宽还是高
- 分辨率：屏幕上物理像素的总数。
- 密度无关像素 (dp)： px = dp * (dpi / 160)。

## [适配不同的系统版本](https://developer.android.google.cn/training/basics/supporting-devices/platforms.html)


*to be continued...*