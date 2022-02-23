<!--
 * @Author: your name
 * @Date: 2022-02-23 14:47:47
 * @LastEditTime: 2022-02-23 14:47:48
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \git\GitignoreConfiguration.md
-->
## .gitignore 配置
>使用gitignore可以忽略一些不需要上傳的文件，使得這些文件不被git識別和追蹤，也部會被上傳到github被別人看到

>### 選擇忽略的文件原則：
> 1. 忽略系統自動生成的文件，EX：縮圖
> 2. 忽略編譯生成的中間文件，可執行文件等，也就是如果一個文件是通過另一個文件自動生成的，那自動生成的文件就沒必要放到git中，EX：.class文件
> 3. 忽略你自己的帶有敏感信息的配置文件，比如存放口令的配置文件


>### .gitignore 文件的格式規範
>* 所有空行或者以 # 開頭的行都會被git忽略
>* 可以使用標準的glob模式匹配
>* 匹配模式可以以(/)開頭防止遞歸
>* 匹配模式可以以(/)結尾指定目錄
>* 要忽略指定模式以外的文件或目錄，可以在模式前加上驚嘆號取反
    