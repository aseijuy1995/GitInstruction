# GitInstruction
Git指令

Git設定\
    更新(Window)	git update-git-for-windows\
    安裝路徑(Window)	where git\
    設定參數	git config\
    設定全域使用者名稱	git config --global user.name "<userName>"\
    設定全域使用者郵件	git config --global user.email "<userEmail>"\
    檢視設定	git config --list\
    檢視設定值	git config <key>\
    說明	git <verb> --help\
    HTTP憑證儲存	git config --global credential.helper cache\
    刪除設定值	git config --global --unset <key>\
    打包成ZIP檔(tar數據文件)	git archive --format=zip --output=<fileName>.tar HEAD\

Git基礎\
    初始化專案	git init\
    檢視目前檔案狀態	git status\
    簡潔顯示狀態資訊	git status -s\
    追蹤新檔案	git add(. / --all)\
    檢視暫存和未暫存的變更	git diff\
    檢視上一次遞交與暫存內容的差異	git diff( --staged / --cached)\
    遞交變更	git commit -m <committed>\
    跳過暫存區將已修改過的檔案遞交變更	git commit -am <committed>\
    遞交變更並顯示相關資訊(分支/SHA-1/增減統計資訊)	git commit -v -am <committed>\
    移除檔案	git rm -f <fileName>\
    從暫存區移出檔案	git rm --cached <fileName>\
    移動檔案 	git mv <file_go> <file_to>\


