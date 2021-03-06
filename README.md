# Number Picker

The android library that provides a simple and customizable NumberPicker.

[![Platform](http://img.shields.io/badge/platform-android-brightgreen.svg?style=flat)](http://developer.android.com/index.html) [![Language](http://img.shields.io/badge/language-java-orange.svg?style=flat)](http://www.oracle.com/technetwork/java/javase/downloads/index.html) [![License](http://img.shields.io/badge/license-apache2.0-lightgrey.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0) [![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-NumberPicker-green.svg?style=true)](https://android-arsenal.com/details/1/3718)

<img src="https://github.com/ShawnLin013/NumberPicker/blob/master/screenshot/NumberPicker-Screenshot.png" width="300">

## Usage

#### Java

```java
NumberPicker numberPicker = (NumberPicker) findViewById(R.id.number_picker);

// set divider color
numberPicker.setDividerColor(getResources().getColor(R.color.colorPrimary));
numberPicker.setDividerColorResource(R.color.colorPrimary);

// set formatter
numberPicker.setFormatter(getString(R.string.number_picker_formatter));
numberPicker.setFormatter(R.string.number_picker_formatter);

// set text color
numberPicker.setTextColor(getResources().getColor(R.color.colorPrimary));
numberPicker.setTextColorResource(R.color.colorPrimary);

// set text size
numberPicker.setTextSize(getResources().getDimension(R.dimen.text_size));
numberPicker.setTextSize(R.dimen.text_size);

// set typeface
numberPicker.setTypeface(Typeface.create(getString(R.string.roboto_light), Typeface.NORMAL));
numberPicker.setTypeface(getString(R.string.roboto_light), Typeface.NORMAL);
numberPicker.setTypeface(getString(R.string.roboto_light));
numberPicker.setTypeface(R.string.roboto_light, Typeface.NORMAL);
numberPicker.setTypeface(R.string.roboto_light);
```

#### XML

add `xmlns:app="http://schemas.android.com/apk/res-auto"`

```xml
<com.shawnlin.numberpicker.NumberPicker
    android:id="@+id/number_picker"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:layout_centerInParent="true"
    app:np_width="64"
    app:np_height="180"
    app:np_dividerColor="@color/colorPrimary"
    app:np_formatter="@string/number_picker_formatter"
    app:np_max="59"
    app:np_min="0"
    app:np_textColor="@color/colorPrimary"
    app:np_textSize="@dimen/text_size"
    app:np_typeface="@string/roboto_light" />
```

### Attributes

|attribute name|attribute description|
|:-:|:-:|
|np_dividerColor|The divider color between the numbers |
|np_formatter|The formatter of the numbers|
|np_max|The max value of the number picker|
|np_min|The min value of the number picker|
|np_textColor|The text color of the numbers|
|np_textSize|The text size of the numbers|
|np_typeface|The typeface of the numbers|
|np_width|The width of the number picker|
|np_height|The height of the number picker|

## Gradle

Add the dependency in your `build.gradle`

```groovy
buildscript {
    repositories {
        jcenter()
    }
}

dependencies {
    compile 'com.shawnlin:number-picker:1.0.1'
}
```

## License

```
Copyright (C) 2016 ShawnLin013(Shawn Lin)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
