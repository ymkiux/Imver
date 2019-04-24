# titlebar  [![](https://jitpack.io/v/ymkiux/Imver.svg)](https://jitpack.io/#ymkiux/Imver)
一个简单易用的导航栏TitleBar库

#### 集成步骤

Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.ymkiux:Imver:Version'
	}
#### 具体使用

Add for the parent node in the required layout.

	<zn.cososk.immerseview</br>
  		android:id="@+id/title_bar"</br>
      	android:layout_width="match_parent"</br>
  		android:layout_height="wrap_content"</br>
      	app:title="默认的标题栏" />

Assignment of state for instantiation of required activities.

	final Imver titleBar = (Imver) findViewById(R.id.title_bar);
	titleBar.setBackgroundColor(Color.parseColor("#ffc9cd"));
	titleBar.setLeftText("返回");
	titleBar.setLeftTextColor(Color.WHITE);
