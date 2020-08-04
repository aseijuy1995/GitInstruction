# GitInstruction
Git指令

Git設定
    更新(Window)	git update-git-for-windows
    安裝路徑(Window)	where git
    設定參數	git config
    設定全域使用者名稱	git config --global user.name "XXX"
    設定全域使用者郵件	git config --global user.email "XXX@gmail.com"
    檢視設定	git config --list
    檢視設定值	git config <key>
    說明	git <verb> --help
    HTTP憑證儲存	git config --global credential.helper cache
    刪除設定值	git config --global --unset <key>
    打包成ZIP檔(tar數據文件)	git archive --format=zip --output=<fileName>.tar HEAD
