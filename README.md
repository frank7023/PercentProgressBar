# PercentProgressBar
[![API](https://img.shields.io/badge/API-15%2B-blue.svg?style=flat)](https://android-arsenal.com/api?level=15) 
[![](https://jitpack.io/v/love-311/PercentProgressBar.svg)](https://jitpack.io/#love-311/PercentProgressBar)
<div align=center>
       <img src="https://github.com/love-311/PercentProgressBar/blob/master/img/img1.png">
</div>

## Prerequisites

Add this in your root `build.gradle` file (**not** your module `build.gradle` file):

```gradle
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

## Dependency

Add this to your module's `build.gradle` file (make sure the version matches the JitPack badge above):

```gradle
dependencies {
	...
	 compile 'com.github.love-311:PercentProgressBar:1.0'
}
```

## Use
A simple in xml:
```xml
 <www.lee311.percentprogressbar.PercentProgressBar
        android:id="@+id/percent_progress_bar"
        android:layout_width="368dp"
        android:layout_height="205dp"
        app:bgColor="@color/red"
        app:iconBitmap="@mipmap/transfer_icon_handle"
        app:iconPadding="20dp"
        app:progressColor="@color/green"
        app:progressMax="100"
        app:progressOrientation="horizontal"
        app:progressValue="0"/>
```

## Method

to set the total value:
```java
mPercentProgressBar.setTotal(329990);
```

to set current progress:
```java
mPercentProgressBar.setProgress(30);
```

to set the text size:
```java
mPercentProgressBar.setTextSize(64);
```

to set the text color:
```java
mPercentProgressBar.setTextColor(getResources().getColor(R.color.colorPrimary));
```
to set the listener of the progress chanage:
```java
mPercentProgressBar.setChangedListener(new PercentProgressBar.OnProgressChangedListener() {
            @Override
            public void onProgressChanged(int currentValue, int percent) {
                
            }
        });
```
