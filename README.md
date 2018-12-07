# FlipView

FlipView is a ViewGroup widget added into the android platforms that will animate a picture by adding 2 different views of the picture on it. The main feature of the FlipView is rotating a picture when it is touched. The animation can contain different styles of pictures, colors, and styles depending on how the user utilizies the FlipView widget. Any number of views can be added in a single layout also depending on the user. The purpose of this component is to add different styles of ImageViews in one layout, while customizing it with animation cycles.

The following are commonly used for FlipView:

- Web View(s)
- List View(s)
- Grid View(s)
- Linear Layout(s)
- Relative Layout(s)
- Table Layout(s)
- Frame Layout(s)

Both FlipView and ViewGroup classes will always be a necessity to create views and layouts in android applications.

## History

The FlipView (in this case regarding the ViewGroup widget) was relased in API level 1, making this widget one of earliest tools to arrive in the android application platform. Throughout the later API levels, different versions of the FlipView widget were created and customized.

Different versions of FlipView include:

- AdapterViewAnimator (API 11)
- AdapterViewFlipper (API 11)
- EasyFlipView (API 15)
- ViewGroupOverlay (API 18)

All of these versions serve the same function and purpose. However, certain libraries need to be installed and imported in the android application as they have to meet their own requirements in order to function by the developer.

## Methods and Attributes

In order to use the FlipView functionality, a library was installed and imported into the app. Inside the build.gradle (Module: app) file, wajahatkarim3's FlipView was used.

```
dependencies {
  implementation 'com.wajahatkarim3.EasyFlipView:EasyFlipView:1.0.0'
}
```
To use the library in the program, you would need to implement the wajahatkarim3's easyflipview library from the build.gradle file. This is the activity_main.xml file.

```
<com.wajahatkarim3.easyflipview.EasyFlipView
...>

</com.wajahatkarim3.easyflipview.EasyFlipView>
```

To get the Image to recognize its going to get flipped, this line of code was added to enable the flip feature on the ImageView.

```
app:flipEnabled="true"
```

In order to make the Image flip when its touched, the following code added a feature to flip the image when touched.

```
app:flipOnTouch="true"
```

To calculate the time the ImageView would be flipped, this attribute was added to determine the duration of the flip in milliseconds. This line of code basically gets the speed of the image while in animation.

```
app:flipDuration="400"
```

## Example Project

In this repository is an example application of how this widget and code functions and works for the user. Not all code is necessary to get the program running. There are basic steps to get the main functionality of the app, however if more features want to be added, more methods and attributes would need to be added for the animation cycle. Althought not mandatory, a landscape .xml file <b> CAN </b> be created to allow full functionality when the screen would be rotated.

There are 3 main functions for the application to run.

```
1. Implement the given library in order to use its functionalities (this is found in the build.gradle (Module: app)).
2. Add the 3 main attributes to get the flip on touch feature running.
3. Import AT LEAST 2 pictures less than 4k resolution to add into the drawable folder.
```

The main function of this widget does not require any coding within the MainActivity.java file. The only files required are the build.gradle file to implement the library, the activity_main.xml file for adding attributes to the FlipView, and the drawable folder was used to add at least 2 pictures.

## References

https://github.com/wajahatkarim3/EasyFlipView

https://github.com/davideas/FlipView

https://developer.android.com/reference/android/view/ViewGroup
