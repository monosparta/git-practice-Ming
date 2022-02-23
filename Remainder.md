<!--
 * @Author: your name
 * @Date: 2022-02-23 14:51:16
 * @LastEditTime: 2022-02-23 14:51:16
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\Remainder.md
-->

## git 進階指令
> <code> git gc </code>
><br>
>手動將過期且不被使用的物件清除掉

> <code> git fsck </code>
><br>
> 檢查Git維護的檔案系統是否完整

> <code> git hash-object </code>
><br> 
> 計算出Blob的SHA1的值
<hr>


## advanced concepts and tools
>1. 不要一次add所有檔案，盡量add更改的目錄或檔案名稱
>>讓你的git commit對應的改便更容易被理解，快速快速掌握最新動態
>2. 完美的Commit Message
>> * subject=簡單摘要發生了什麼事
>> - Body
>>      - 與前者的不同
>>      - 更改的理由
>>      - 有任何需要注意或哪邊更改更好的嗎？ 
>3. 與團隊達成共通的約定
>>  - 始終整合在主要的發展分支上
>>  - 可參考一些已經規定好的規範如：Gitflow


## 雜紀錄

> ### git add . V.S. git add -all 的差別
><b> -all 是不管專案的哪一層皆會作用 <br> . 為執行檔案的同一層以及子目錄作用</b>

