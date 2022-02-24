<!--
 * @Author: your name
 * @Date: 2022-02-23 15:17:21
 * @LastEditTime: 2022-02-24 10:39:12
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\Girflow.md
-->

# GitFlow 介紹
> ## 1.Git Flow
> 根據建議主要分支有：master、develop、hotfix、release與feature
>
<br>

<img src="pic/flow.png">

>### <b>Master分支</b>
>主要用來放穩定、確定要上線的版本。通常此分支的來源是從別的分支合併過來，開發者不會直接Commit到這個分之。由會是穩定版本，因此通常這個分支上的Commit會打上的版本號標籤。

>### <b>Develop分支</b>
>主要是所有開發的基礎分支，當要新增功能時，所有的Feature分支都是會從這個分支切分出去的，完成的feature分支也會合併過來這個分支。

>### <b>Feature分支</b>
>當要開始新增功能的時候，便可以使用Feature分支，大多都是從Develop分支出來的，feature分支回併到Develop分支的過程通常都會搭配Code Review，也確認程式碼的測試有通過

>### <b>Hotfix分支</b>
>當線上的產品發生緊急問題時，會從Master分支開一個Hotfix分支出來進行修復，Hotfix分支修復完後，會合併回Master分支，同時合併一分到Develop分支。
>### <b>Release分支</b>
>當認為Develop分支夠成熟了，就可以把Develop分支合併到Release分支，在這邊進行算是上線前的最後測試。測試完成後會同時合併到Master分支與Develop這兩個分支上。同步到Develop分支的目的，是因為可能在Release分支上還會測到並修正一些問題，所以需要跟Develop分支同步。
> 通常Release分支上會進行更完善的原始碼測試、修正預備釋出版本等動作。



>## 總結

>> |  | Git flow | GitHub flow |Gitlab flow |
>> | -------- | -------- | -------- |-------- |
>> | 優點     | 清晰可控   | 適合持續發布的類型    |  Gitflow與Github folw的綜合    |
>> | 缺點     | 複雜且需要頻繁的切換分支  |  master是最新代碼但準備發布的版本卻不一定是最新代碼<br>或是固定時間才發布更新的項目就會有影響   | ？  |
>> | 需注意   | 版本快速更換的專案中Hotfix和Release分支很少用 <br>如果有啟用這兩個分支的話需要記得合併回去develop與master分支 |如果只有一個master會不夠用，需要另外再建立一個新分支維護   |  增加了prodution分支為專門發布版本

<hr>