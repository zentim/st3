# 同步 Sublime Text 3 配置
需要同步的是 Packages 目錄下的 User 目錄。

## 有些文件不需要同步，加入到 .gitignore
```
Package Control.last-run
Package Control.ca-list
Package Control.ca-bundle
Package Control.system-ca-bundle
Package Control.cache/
Package Control.ca-certs/
```

## 尋找 Packages 目錄的位置
* Sublime Text3: ``` Preferences -> Browse Packages ```
* Windows: ``` %APPDATA%\Sublime Text 3\Packages ```
* Linux: ``` ~/.config/sublime-text-3/Packages ```

-----

## Quick Start
1. 開啟 sublime text 並安裝 package control (參考 https://packagecontrol.io/installation)
2. 進入 Packages 目錄 (Preferences -> Browse Packages) 下並刪除 User 目錄
3. 在 Packages 目錄下 clone 遠端 repo 並重命名為 User:
```
git clone https://github.com/zentim/st3.git User
```
4. 重啟 sublime text，按 ``` Ctrl + ` ``` 可以查看 plugin 安裝狀態，如果有錯誤則重啟，可能需要重複多次

-----

## 從遠端同步到本地
進入 Packages 目錄:
```
git pull
```

## 從本地同步到遠端
進入 Packages 目錄:
```
git add . 
git commit -m "Update settings"
git push
```
