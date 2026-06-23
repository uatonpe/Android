ANIK One Desk Android App - Build Guide

या ZIP मध्ये तुमचा updated HTML portal WebView Android app मध्ये ठेवला आहे.
Password save / auto sign-in / localStorage same राहील कारण WebView मध्ये JavaScript + DOM Storage enable आहे.

Build करण्यासाठी:
1) Android Studio install/open करा.
2) File > Open > ANIK_One_Desk_Android_App folder निवडा.
3) Gradle sync complete होऊ द्या.
4) Build > Build Bundle(s) / APK(s) > Build APK(s).
5) APK path: app/build/outputs/apk/debug/app-debug.apk

Release APK साठी:
Build > Generate Signed Bundle / APK > APK > key तयार करा > release build करा.

महत्त्वाचे:
- App ID: com.anik.onedesk
- App name: ANIK One Desk
- Internet, Camera, Storage permissions added आहेत.
- Local HTML: app/src/main/assets/index.html
- API URL HTML मध्ये आधीसारखाच आहे.
- Logout button वापरल्यास HTML code localStorage मधील saved password remove करतो.

जर Android Studio मध्ये androidx.core dependency error आला तर app/build.gradle मध्ये dependencies add करा:
dependencies { implementation 'androidx.core:core:1.13.1' }

किंवा FileProvider नको असल्यास camera upload support remove करावा लागेल. Camera/file upload support साठी dependency लागते.
