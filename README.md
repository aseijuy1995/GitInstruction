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
    打包成ZIP檔(tar數據文件)	git archive --format=zip --output=<fileName>.tar HEAD

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
    移動檔案 	git mv <file_go> <file_to>

Git歷史紀錄\
    檢視遞交歷史 	git log\
    檢視遞交歷史並顯示遞交差異 	git log -p\
    檢視遞交歷史並簡要統計資訊	git log --stat\
    檢視遞交歷史並更改輸出格式	git log --pretty=<verb>  (oneline / shoort / full / fuller)\
    檢視遞交歷史並自訂輸出格式	git log --pretty=format:"<formatDesc>"\
    檢視遞交歷史並顯示ASCII基本圖表	git log --graph\
    檢視遞交歷史並顯示更改檔案統計資訊	git log --shortstat\
    檢視遞交歷史並顯示有被更改的檔案	git log --name-only\
    檢視遞交歷史並顯示有被更改的檔案與更改過的統計資訊	git log --name-status\
    檢視遞交歷史並簡短顯示SHA-1值	git log --abbrev-commit\
    檢視遞交歷史並顯示相對日期	git log --relative-date\
    檢視遞交歷史並只顯示最新n筆遞交	 git log -(n)\
    檢視遞交歷史並指定日期之後的遞交 	git log --since --after\
    檢視遞交歷史並指定日期之前的遞交	git log --until --before\
    檢視遞交歷史並依名查詢相關遞交 	git log --author="<author>"\
    檢視遞交歷史並依關鍵字查詢相關遞交	git log --grep="<grep>"\
    檢視遞交歷史並依多條件查詢相關遞交	git log --author="<author>" --grep="<grep>" --all-match\
    檢視遞交歷史並指定相符字串的遞交	git log --committer <committer>\
    檢視遞交歷史並依增減相關方法的最後一次遞交	git log -S<funcName>\
    顯示指向此提交的所有引用(分支,標籤等) 	git log --decorate\
    顯示欲合併的遞交清單	git log --no-merges <current_branch_name>..<target_branch_name>\
    顯示引用內容	git log <target_branch_name> --not <current_branch_name>

Git遠端\
    複製遠端專案 	git clone <githubURL>\
    複製遠端專案並重新命名專案	git clone <githubURL> <projName>\
    顯示遠端倉庫	git remote\
    顯示遠端倉庫並顯示對應URL	git remote -v\
    增加遠端倉庫	git remote add <remoteName> <url>\
    從遠端倉庫取得和擷取資料	git fetch <remoteName> <branchName>\
    資料發送到遠端倉庫	git push <remoteName> <branchName>\
    檢查遠端倉庫 	git remote show <remoteName>\
    重新命名遠端倉庫	git remote rename <oldBranchName> <newBranchName>\
    刪除遠端倉庫 	git remote rm <branchName>\

Git標籤\
    列舉標記	git tag\
    註釋標籤	git tag -a \<tagName\> -m "<commend>"\
    顯示標籤資訊	git show \<tagName\>\
    輕量標籤	git tag \<tagName\>\
    補加標籤	git tab -a \<tagName\> <SHA-1>\
    共用標籤	git push origin \<tagName\> / git push origin --tags\
    刪除本地標籤	git tag -d \<tagName\>\
    刪除遠端標籤 	git push origin --delete tag \<tagName\>\
    顯示最近標籤 	git describe \<branchName\>\ 




