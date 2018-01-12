# Bypass Facebook SSL Pinning (REQUIRE ROOTED)
Bypassing Facebook SSL pinning for version 154.0.0.33.385 | Min API 15 | arm | January 11, 2018
[Download Link](https://www.apkmirror.com/apk/facebook-2/facebook/facebook-154-0-0-33-385-release/facebook-154-0-0-33-385-android-apk-download/)


#### libcoldstart.so

Replace the libcoldstart.so file in **/data/data/com.facebook.katana/lib-xzs**



## Steps:



We need to patch **0x001F9B24** and **0x001F9B26**:

![before_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-SLL-Pinning/master/arm/before_patch.jpg?54119)


After patching these offsets to **0xB1C4** and **0xB948**, patched lib should be like this:


![after_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-SLL-Pinning/master/arm/after_patch.jpg?54119)

---



[Refrence](https://serializethoughts.com/2016/08/18/bypassing-ssl-pinning-in-android-applications/) & Thanks for [pouyadarabi](https://github.com/pouyadarabi/Facebook_SSL_Pinning)

