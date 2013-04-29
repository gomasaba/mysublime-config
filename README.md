# 自分用のsublimetext2の設定

windows < > imac <> air で設定を共通するために。

##設定ファイルの場所とハードリンクを貼る

### mac

ハードリンクを貼れるようにする

[https://github.com/selkhateeb/hardlink](https://github.com/selkhateeb/hardlink)

メインでのimacでハードリンクを貼る

	hardlink ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/User ~/mysublime-config/User

サブのairでは逆のハードリンクを貼る（元のUserは一旦リネームして退避）
	hardlink ~/mysublime-config/User/ ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/User


### windows
・macで設定したファイルを持ってくる

ハードリンクを貼る（１ファイルずつ？）

・元の設定ファイルを削除

	C:\Users\ohta\Documents\mysublime-config\User\Preferences.sublime-settings
	C:\Users\ohta\Documents\mysublime-config\User\Preferences.sublime-settings

・ハードリンクを貼る

	mklink /H "C:\Users\ohta\AppData\Roaming\Sublime Text 2\Packages\User\Preferences.sublime-settings" "C:\Users\ohta\Documents\mysublime-config\User\Preferences.sublime-settings"
