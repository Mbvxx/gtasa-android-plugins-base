WILDAN ULTIMATE CHEAT MENU v1.0
GTA San Andreas Android 2.10
Android Mod Loader (AML)
Target ABI: arm64-v8a

FIT
cd ~/gtasa-android-plugins-base

cat > wildan_mod/main.cpp <<'EOF'
#include <jni.h>
#include <android/log.h>

#define LOG_TAG "WildanUltimate"
#define LOGI(...) __android_log_print(ANDROID_LOG_INFO, LOG_TAG, __VA_ARGS__)

extern "C" JNIEXPORT jint JNICALL
JNI_OnLoad(JavaVM* vm, void* reserved) {
    LOGI("Wildan Ultimate Cheat Menu v1.0 loaded!");
    return JNI_VERSION_1_6;
}
