<!--
 * @Author: your name
 * @Date: 2022-02-23 14:49:12
 * @LastEditTime: 2022-02-23 14:49:12
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\AboutCommit.md
-->
## Commit 介紹及使用

>### Commit版控的基本原則
> 在git中大多使用git commit 來建立許多的版本，要有一個好的「版本紀錄」，可以遵從以下原則：
> * 做一個小工能修改就建立版本，容易追蹤變更

> * 千萬不要累積一大堆修改後才建立一個大版本

> * 有邏輯、有順序的修正功能，確保相關的版本修正可以按順序提交（commit），以便追蹤

>### 修正Commit歷史紀錄的理由
>由於git開放每個人都能夠任意的修正Commit歷史紀錄，因此若有人任意竄改版本，會使Git版本控管無法正常運作。但正因為有些情境需要修改版本紀錄，所以Git保留了這樣的機制，希望使用者能在「自我控管版本」到一定的程度後，能有機會整理版本紀錄的各種資訊，讓程式正式發布後他人可以更清楚你版本做了哪一些地修改。
>#### 修改版本歷史紀錄需要特別注意：
>* 一個儲存庫可以有許多分之
>* 分享Git原始碼得最小單位是以「分支」為單位
>* 可以任意修改某個支線上的版本，在你「分享」給其他人前
>* 分享後便不要隨意地再更動了

> #### <code> git reset </code>
><br>
> 可以重製工作目錄與修正版本歷史紀錄

>#### <code> git revert </code>
><br>
> 把某個版本的變更，透過「相反」的步驟把變更給還原

>#### <code> git cherry-pick </code>
><br>
> 一個將要廢棄的分支中手動挑出想要套用的版本變更，重新套用完全的變更




