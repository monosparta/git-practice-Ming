<!--
 * @Author: your name
 * @Date: 2022-02-23 14:46:49
 * @LastEditTime: 2022-02-23 14:46:49
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\GitCommonInstructionSet.md
-->


##  Git 常用指令集介紹

>  <code>git init</code>
><br>
>建立一個Git新的Repository（倉庫）

> <code> git clone </code>
><br>
>複製別人的Repository 當你想要抓別人的程式碼自己修改時

> <code> git status </code>
><br>
>檢查git的狀態

> <code> git add （.）</code>
><br>
>讓檔案能被git追蹤

> <code>git commit -m "" </code>
><br>
>提交檔案，讓你未來可以回溯與追蹤參考

> <code> git log (--stat/-p) </code>
><br>
>查看過去的commit紀錄。--stat是提交詳細內容;--p參數可以看到檔案更詳細的變更內容。

> <code> git rm '檔案名稱' </code>
><br>
>刪除目錄快取的此檔案與工作目錄下的此檔案

> <code> git mv "原先名稱" "新改的名稱" </code>
><br>
>用來變更檔案或目錄的名稱

> <code> git reset　(--hard) </code>
> <br>
>重製目前工作目錄的「索引狀態」，但是是無法拯救已被更動或刪除的檔案或目錄。參數hard可以還原到目前最新版

> <code> git checkout "分支" "檔案名稱" </code>
><br>
>救回被改壞的檔案回溯到沒修改前的版本

> <code> git diff </code>
><br>
>檢視修改內容

> <code> git branch </code>
><br>
>建立分支

> <code> git branch -d </code>
> <br>
>刪掉分支

> <code>git push origin "分支名稱" </code>
> <br>
>把本地端的分支推到遠端

> <code> git rebase "branch" </code>
><br> 
>以某分為基底重接

> <code> git merge （branch）</code>
><br>
>比較兩個檔案後合併分支