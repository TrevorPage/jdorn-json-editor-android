# jdorn-json-editor-android
Evaluation of jdorn's json-editor being used in an Android WebView.

This is a test project to evaluate [Jeremy Dorn's](https://github.com/jdorn) most excellent  [json-editor](https://github.com/jdorn/json-editor) JSON Schema Based Editor being used within a `WebView` in an Android application. It also makes use of other libraries ([jQuery](https://jquery.com/), [Spectrum colour picker](http://bgrins.github.io/spectrum/)) for reasons discussed below.

# Screenshot

![Screenshot](https://github.com/TrevorPage/jdorn-json-editor-android/blob/master/screenshots/screenshot_1.png)

# WebView colour picker problem work-around

The project makes use of [Spectrum](http://bgrins.github.io/spectrum/) to pollyfill in place of the native `<input type="color">` because of the fact that, at least in my experience, the `WebView`'s native colour picker fails to work, crashing with an exception relating to `com.android.org.chromium.ui.ColorPickerAdvanced`. 

Comments in `index.html` explain how I managed to get Spectrum to play nicely with the JSON editor.
