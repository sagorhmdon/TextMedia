# ~~TextMedia~~ / MediaText
This Library for your note application or any kind of rich media Edittext application. You can add image or video or any kind of file add 
into your edittext/MediaText xml file.
for use it use in your root build.gradle
```java
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

and add in your depedience

```java
dependencies {
	  implementation 'com.github.sagorhmdon:TextMedia:1.0'
	}
  ```
  
# Feature and Methods Introduction

- setEditorFontSize(int value); // Font size as your requirement
- setEditorFontColor(Color.GRAY); // Font Color As your requirement
- setPadding(left, top, right, bottom); // you can use padding as you want
- setPlaceholder("Your text here..."); // you can set hint using this method

# Media Method

- insertImage("link","alt"); // insert image in cursor position
- insertVideos("link","name"); // insert video in cursor position

** lets get back html 

 ```java
 setOnTextChangeListener(new MediaText.OnTextChangeListener() {
            @Override public void onTextChange(String text) {
                //text will give you html code
	
            }
        });
 ```
 
 Happy coding
