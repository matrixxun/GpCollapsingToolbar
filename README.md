# GooglePlay-CollapsingToolbar
Extended CollapsingToolbar that implemented scrolling behaviour like in Google Play app
![](https://raw.githubusercontent.com/VyacheslavShmakin/GpCollapsingToolbar/master/sample/demo.gif)


Download
--------

Gradle:

```groovy
compile 'com.github.VyacheslavShmakin:gp-collapsing-toolbar:1.0.1'
```

Maven:

```xml
<dependency>
    <groupId>com.github.VyacheslavShmakin</groupId>
    <artifactId>gp-collapsing-toolbar</artifactId>
    <version>1.0.1</version>
    <type>aar</type>
</dependency>
```


Usage
-----
#### In Code
If you wanna enable/disable or check like Google Play app styled behaviour programmatically you should call these methods
``` java
myGpCollapsingToolbar.setGooglePlayBehaviour(true);
myGpCollapsingToolbar.isGooglePlayBehaviour();
```

-----
#### In xml

You should use the same parameters that defined in support.design library for CollapsingToolbar with "gp_" prefix
```xml
<ru.shmakinv.android.material.widget.GpCollapsingToolbar
            android:id="@+id/toolbar_layout"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:fitsSystemWindows="true"
            app:gp_collapsedTitleTextAppearance="@style/Toolbar.TitleText"
            app:gp_marketStyledBehaviour="true"
            app:gp_contentScrim="@color/color_primary"
            app:gp_scrimAnimationDuration="300"
            app:layout_scrollInterpolator="@android:anim/accelerate_decelerate_interpolator"
            app:layout_scrollFlags="scroll|enterAlways|enterAlwaysCollapsed"
            app:gp_statusBarScrim="@color/color_primary_dark"
            app:toolbarId="@id/toolbar">
            ...
</ru.shmakinv.android.material.widget.GpCollapsingToolbar>
```
