# Another thread management in Android
https://codelabs.developers.google.com/codelabs/kotlin-android-training-complex-lifecycle/index.html#2

> Compile and run the app, and click the Home button after the timer starts. Even though the app is in the background, the timer is running, and continually using system resources. Having the timer continue to run is a memory leak for your app, and probably not the behavior you want.

> The general pattern is that when you set up or start something in a callback, you stop or remove that thing in the corresponding callback. This way, you avoid having anything running when it's no longer needed.

