<!--
 * @Author: your name
 * @Date: 2022-02-23 14:48:30
 * @LastEditTime: 2022-02-23 14:48:30
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\Howtousebranches.md
-->
## 分支的使用方法
> 在版本控制中的分支「機制」，主要目的是為了解決開發過程中版本衝突的問題，然而同時也不少的版本問也是因為開始使用分支後而產生的。
>是指向某個commit的指標

### 分支的基本指令
> <code> git branch "分支名稱" </code>
><br>
>建立一個分支

> <code> git checkout -b "已有分支名稱" </code>
><br>
>將目前工作目錄切換到已有的分支

> <code> git checkout -b "新的分支名稱"</code>
><br>
>建立一個新得分支並切換到新的分支

> <code> git branch -d "分支名稱"</code>
><br>
>刪除分支

### 分支合併操作-merge篇 
> merge的合併方式分為fast-forward 和 no-fast-forward，下面有小動圖可以快速比較

#### <code>git merge "分支" </code>

>git 預設會以 fast-forward 的模式進行合併

<img src="pic/merge_fast_foard.gif">
<br>

> [Gif 來源：CS Visualized](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1#merge)
> 

#### <code>git merge "分支" --no-ff</code>

>能清楚的知道是由哪一個分支進行合併

<img src="pic/merge_no_fast_forward.gif">
<br>

> [Gif 來源：CS Visualized](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1#merge)
> 
```
因此我們可以fast-forward 用來 merge 些較不重要的 commit，使用merge_no_fast_forward模式合併則是在重要的更改時
```
### 分支合併操作-rebase篇 
> 1. 合併版本
>> rebase顧名思義就是重新修改特定分支的「基礎版本」，把另一個分支的變更當成我這個分支的基礎

> #### <code>git rebase "分支"</code>
>進行Rebase動作，把master當成我們的基礎版本

<img src="pic/git_rebase.gif">
<br>

> [Gif 來源：CS Visualized](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1#merge)
> 

>2. 修改歷史 commit 紀錄





> #### <code>git rebase -i HEAD~3</code>
>

<img src="pic/git_rebase_i.gif">
<br>

> 還可以修改特定分支上任何一個版本的版本資訊

```
 rebase 會改變歷史紀錄，因此使用的時候要注意有沒有也在使用這個分支
```

>[Gif 來源：CS Visualized](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1#merge)
> 

>### 使用時機總結
>  branch 是私有分支，rebase 可以有效幫你「重整版本」來保持 commit 紀錄是呈線性整齊，而如果是共有分支則使用 merge fast-forward 或 merge no–fast-forward，來避免修改到同事的歷史紀錄。
<hr>
