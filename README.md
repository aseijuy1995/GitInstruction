# GitInstruction
Git指令

Git設定 \
    更新(Window)	git update-git-for-windows \
    安裝路徑(Window)	where git \
    檢視指令	git config \
    設定全域使用者名稱	git config --global user.name "\<name\>" \
    設定全域使用者郵件	git config --global user.email "\<email\>" \
    檢視設定	git config --list \
    檢視設定值	git config \<key\> \
    說明	git \<verb\> --help \
    HTTP憑證儲存	git config --global credential.helper cache \
    刪除設定值	git config --global --unset \<key\> \
    打包成ZIP檔(tar數據文件)	git archive --format=zip --output=\<file_name\>.tar HEAD \
    Git別名/替換Git別名	git config --global alias.\<abbrev\> \<full_name\> \
    刪除Git別名	git config --global --unset alias.\<abbrev\>

Git基礎 \
    初始化專案	git init \
    檢視目前檔案狀態	git status \
    簡潔顯示狀態資訊	git status -s \
    追蹤新檔案	git add(. / --all) \
    檢視暫存和未暫存的變更	git diff \
    檢視上一次遞交與暫存內容的差異	git diff( --staged / --cached) \
    檢查遞交前存在的空白錯誤	git diff --check \
    顯示分支並合併差異點	git diff \<current_branch\>...\<target_branch\> \
    遞交變更	git commit -m \<commit\> \
    跳過暫存區將已修改過的檔案遞交變更	git commit -am \<commit\> \
    遞交變更並顯示相關資訊(分支/SHA-1/增減統計資訊)	git commit -v -am \<commit\> \
    重設上一次遞交的作者信息 	git commit --amend --reset-author \
    取消操作並重新修改commit名	git commit -m "\<commit\>" --amend \
    移除檔案	git rm -f \<file_name\> \
    從暫存區移出檔案	git rm --cached \<file_name\> \
    移動檔案 	git mv \<file_from\> \<file_to\> \
    取消已暫存的檔案 	get reset head \<file_name\> \
    取消已修改的檔案	git checkout -- \<file_name\>

Git歷史紀錄 \
    檢視遞交歷史 	git log \
    檢視遞交歷史並顯示遞交差異 	git log -p \
    檢視遞交歷史並簡要統計資訊	git log --stat \
    檢視遞交歷史並更改輸出格式	git log --pretty=\<verb\>  (oneline / shoort / full / fuller) \
    檢視遞交歷史並自訂輸出格式	git log --pretty=format:"\<format_desc\>" \
    檢視遞交歷史並顯示ASCII基本圖表	git log --graph \
    檢視遞交歷史並顯示更改檔案統計資訊	git log --shortstat \
    檢視遞交歷史並顯示有被更改的檔案	git log --name-only \
    檢視遞交歷史並顯示有被更改的檔案與更改過的統計資訊	git log --name-status \
    檢視遞交歷史並簡短顯示SHA-1值	git log --abbrev-commit \
    檢視遞交歷史並顯示相對日期	git log --relative-date \
    檢視遞交歷史並只顯示最新n筆遞交	 git log -(n) \
    檢視遞交歷史並指定日期之後的遞交 	git log --since --after \
    檢視遞交歷史並指定日期之前的遞交	git log --until --before \
    檢視遞交歷史並依名查詢相關遞交 	git log --author="\<author\>" \
    檢視遞交歷史並依關鍵字查詢相關遞交	git log --grep="\<grep\>" \
    檢視遞交歷史並依多條件查詢相關遞交	git log --author="\<author\>" --grep="\<grep\>" --all-match \
    檢視遞交歷史並指定相符字串的遞交	git log --committer \<committer\> \
    檢視遞交歷史並依增減相關方法的最後一次遞交	git log -S\<func_name\> \
    顯示指向此提交的所有引用(分支,標籤等) 	git log --decorate \
    顯示欲合併的遞交清單	git log --no-merges \<current_branch\>..\<target_branch\> \
    顯示引用內容	git log \<target_branch\> --not \<current_branch\>
    檢視各分支所指向的物件	git log --oneline --decorate

Git遠端 \
    複製遠端專案 	git clone \<url\> \
    複製遠端專案並重新命名專案	git clone \<url\> \<proj_name\> \
    顯示遠端倉庫	git remote \
    顯示遠端倉庫並顯示對應URL	git remote -v \
    增加遠端倉庫	git remote add \<remote_name\> \<url\> \
    從遠端倉庫取得和擷取資料	git fetch \<remote_name\> \<branch_name\> \
    資料發送到遠端倉庫	git push \<remote_name\> \<branch_name\> \
    檢查遠端倉庫 	git remote show \<remote_name\> \
    重新命名遠端倉庫	git remote rename \<old_branch\> \<new_branch\> \
    刪除遠端倉庫 	git remote rm \<branch\> \
    資料發送到遠端覆蓋當前遠端 	git push -f \<current_branch\> \<remote_branch\>

Git標籤 \
    列舉標記	git tag \
    註釋標籤	git tag -a \<tag\> -m "\<commit\>" \
    顯示標籤資訊	git show \<tag\> \
    輕量標籤	git tag \<tag\> \
    補加標籤	git tab -a \<tag\> \<SHA-1\> \
    共用標籤	git push origin \<tag\> / git push origin --tags \
    刪除本地標籤	git tag -d \<tag\> \
    刪除遠端標籤 	git push origin --delete tag \<tag\> \
    顯示最近標籤 	git describe \<branch\>

Git分支機制 \
    建立分支	git branch \<branch\> \
    刪除分支 	git branch -d \<branch\> \
    切換分支 	git checkout \<branch\> \
    建立並切換至分支	git checkout -b \<branch\> \
    檢視已合併過的分支	git branch --merged \
    檢視未合併的分支 	git branch --no-merged \
    建立追蹤分支	git checkout -b \<branch\> \<remote\>/\<remote_branch\> \
    建立追蹤分支	git checkout --track \<remote\>/\<remote_branch\> \
    更改遠端追蹤分支	git branch -u \<remote\>/\<remote_branch\> \
    檢視設定的追蹤分支	git branch -vv \
    刪除遠端分支	git push \<remote\> --delete \<branch\>

Git合併 \
    合併分支	git merge \<branch_name\> \
    合併遠端分支	git merge @{u} \
    接受以合併分支其壓縮成一個變更	git merge --squash \<target_branch\>

Git變基 \
    基本變基合併 	git rebase \<target_branch\> \
    衍生變基合併	git rebase --onto \<target_branch\> \<center_branch\> \<current_branch\> \
    揀選需要的紀錄作為合併主分支中(類似rebase) 	git cherry-pick \<SHA-1\>






