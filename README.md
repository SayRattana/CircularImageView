# CircularImageView
[![](https://jitpack.io/v/SayRattana/CircularImageView.svg)](https://jitpack.io/#SayRattana/CircularImageView)


CircularImageView to show your images in Circular Shape.
* min SDK 19 (Android 4.4 KitKat)
* written in Java

A lightweight and fully customizable library to show your images in Circular Form

## Screenshots
<div align="center">
    <img src="https://github.com/SayRattana/CircularImageView/blob/master/screenshots/screen1.png" width="300px"</img> 
    <img src="https://github.com/SayRattana/CircularImageView/blob/master/screenshots/screen2.png" width="300px"</img> 
</div>

## Installation

Add this into your root build.gradle file:

```java
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
Add the dependency to your module build.gradle:
```java
dependencies {
	         implementation 'com.github.SayRattana:CircularImageView:1.0.0'
}
```
## Usage
### Using XML Layout
```xml
<com.rattanasay.circularimageviewlib.CircularImageView
        android:id="@+id/imageView"
        android:layout_width="200dp"
        android:layout_height="200dp"
        android:layout_centerHorizontal="true"
        android:src="@drawable/profile_pic"
        app:c_background_color="@color/colorPrimary"
        app:c_border="true"
        app:c_border_color="#4A97E4"
        app:c_border_width="2.5dp"
        app:c_shadow="true"
        app:c_shadow_color="#000"
        app:c_shadow_gravity="end"
        app:c_shadow_radius="2.5" />
```
### Programatically
```java
CircularImageView circularImageView = findViewById(R.id.imageView);
circularImageView.setImageResource(R.drawable.profile_pic);
circularImageView.setBackgroundColor(getResources().getColor(R.color.colorPrimary));
circularImageView.setBorderWidth(5);
circularImageView.setBorderWidth(10);
circularImageView.setBorderColor(getResources().getColor(R.color.colorPrimaryDark));
circularImageView.setShadowGravity(CircularImageView.ShadowGravity.BOTTOM);
circularImageView.setShadowRadius(9);
```



