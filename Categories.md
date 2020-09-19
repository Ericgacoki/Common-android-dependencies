## Image loading

1. ## [Glide](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwikoaX5kPbrAhUFrxoKHcQeB8IQFjAAegQIAxAB&url=https%3A%2F%2Fgithub.com%2Fbumptech%2Fglide&usg=AOvVaw0fHFdq84xxgrLwKnRikfpc)

Glide is a powerful image loading tool that has a bunch of advantages over other image loaders. 
To add Glide in to your project, do the followi
```Kotlin

//first ensure you have maven and google repositories.Add the followind to build.gradle file

repositories {
  mavenCentral()
  google()
}

// add glide repository in the gladle module app file

dependencies {
  implementation 'com.github.bumptech.glide:glide:4.11.0'
  annotationProcessor 'com.github.bumptech.glide:compiler:4.11.0'
}

//Usage (I'm assuming you're using Kotlin)

GlideApp
  .with(this)
  .load("https://www.shutterstock.com/image-photo/kiev-ukraine-may-26-2015-android-283385381")
  .into(imageView)

