# ADB

## Show connected device

`./adb devices`

## Show address of the app Todolist in Android

`./adb shell pm list packages | grep todolist`

## Install .apk file of the app Todolist via ADB

`./adb install '/c/Program Files/ADB_android/TodoList.apk'`

## Make a screenshot of Todolist and copy it, using one command

`./adb shell screencap /storage/emulated/0/DCIM/screen.png && ./adb pull /storage/emulated/0/DCIM/screen.png screen.png`

## Show console logs of the app Todolist

`./adb logcat | grep com.android.todolist`

## Copy logs on your computer

`./adb logcat | grep com.android.todolist >  '/c/Program Files/ADB_android/logs1.txt'`

## Delete the app Todolist from the phone using ADB

`./adb uninstall com.android.todolist`
