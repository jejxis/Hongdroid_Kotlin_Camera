# Hongdroid_Kotlin_Camera
카메라 이용/ 출처: https://www.youtube.com/watch?v=inprJiLDUIU&amp;list=PLC51MBz7PMywN2GJ53aF0UO5fnHGjW35a&amp;index=9&amp;ab_channel=hongdroid%ED%99%8D%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C

(2022.3.16 기준) PermissionListener 에러=> 
build.gradle(:app)에서
dependencies{... implementation 'io.github.ParkSangGwon:tedpermission:2.3.0' ...}
2021년 7월에 2.3.0으로 변경되었다고 함.
출처: https://link2me.tistory.com/1823

그 외 여러가지 에러
Exception 'open failed: EACCESS (Permission denied)'=> 
AndroidManifest.xml에서
<application... android:requestLegacyExternalStorage="true" ...>
출처: https://stackoverflow.com/questions/8854359/exception-open-failed-eacces-permission-denied-on-android

Duplicate class android.support.v4.app.InotificationSideChannel found in modules classes=> 
gradle.properties에서
android.useAndroidX=true
android.enableJetifier=true
출처: https://stackoverflow.com/questions/55909804/duplicate-class-android-support-v4-app-inotificationsidechannel-found-in-modules
