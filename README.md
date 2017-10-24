# 同步 Sublime Text 3 配置
需要同步的是 Packages 目錄下的 User 目錄。

## Init Step
1. 開啟 sublime text 並安裝 package control (參考 https://packagecontrol.io/installation)
2. 進入 packages 目錄 (Preferences -> Browse Packages) 下並刪除 User 目錄
3. 在該目錄下 git clone
4. 重啟 sublime text，``` Ctrl + ` ``` 查看 plugin 安裝狀態，如果有錯誤則重啟，可能需要重複多次

## Packages 目錄的位置
* Sublime Text3: ``` Preferences -> Browse Packages ```
* Windows: ``` %APPDATA%\Sublime Text 3\Packages ```
* Linux: ``` ~/.config/sublime-text-3/Packages ```
