# RLadies 要上 Github 
By Rachael Pai 2017/03/27

![](https://i.imgur.com/ncbIdKF.png)

---

## 為何 RLadies 要上 Github ? 

+ 因為每次的 RLadies meetings 都很精彩，source code 與文件想要分享給更多人
+ 因為 RLadies 有很多工作小組， 工作小組成員間要互相協作產出文件或 source code
+ 因為我們希望記錄下每一個人的貢獻
+ 因為我們希望分享的 source code 有歷史紀錄，可以回復也可以更新



---

## 甚麼是 Github 呢 ?

那麼要先了解什麼是 Git ? 

---

## 甚麼是 Git 呢? 

+ Distributed Version Control System / 分散式版本控制系統
+ 檔案系統快照資料庫/倉庫的管理系統
+ 資料庫 : Repository


---

## 甚麼是 Github 呢 ?
+ Wiki : GitHub是一個透過Git進行版本控制的軟體原始碼<B> 代管服務</B>
+ https://github.com/

+ 提供 Git 的雲端服務的網站

---

## 如何開始第一步 ?

----

## 在 Github 上申請帳號

+ github.com

----

## 安裝 Git 到本地電腦

有以下太太太簡單的安裝方法 

+ ubuntu
    apt-get install git
+ linux
    yum install git 
+ mac 
    bew install git 
+ windows 
    下載安裝檔, run exe 檔
+ 或者請參考 Git 官網
https://git-scm.com/book/zh-tw/v1/%E9%96%8B%E5%A7%8B-%E5%AE%89%E8%A3%9DGit

---

## 開始 RLadies Github 的情境教學

---

## 情境1 : 我參加了 RLadies 聚會， RBasic 教材太棒惹，我想要下載教材

----

+ 請上 Github (https://github.com/)
+ 搜尋 rladiestaipei , 進入 rladiestaipei/R-basic
+ copy clone 位址
+ 在 command line 下 (ie. git bash)
    ```
    git clone https://github.com/rladiestaipei/R-basic.git
    ```
+ 你有了一份完整 R-basic Repository 的本地目錄了
+ 你會發現 R-basic 教材都在你的本地電腦了

---

## 情境2 : 我是 RBasic 工作小組成員，我要參加 RBasic 共同編輯

----

## Git 的 3 個 states

+ Modified (修改): 檔案有修改，但還沒commit 到本地資料庫
+ Staging (已暫存): 幫檔案照快照
+ Committed (已提交) : 檔案已經安全存放在你本地的資料庫


----

## Git 基本工作流程

+ 取出某個版本的檔案 (from Repository) 
+ -> 修改檔案 
+ -> 儲存 Stage 快照到 Staging Area 
+ -> Commit 到Git 資料庫 (to loacl Repository)

----


![](https://i.imgur.com/d2jbJOl.png)

----

## 提交到遠端資料庫 (Remote)
+ Remote 這邊是指 github 上的 repository . 
+ Remote 也可以是 gitlab, bitbucket 等

----

R-Basic 共編 git 實作

----

+ 先跟情境1 一樣 clone 下你的目錄，擁有一份 Local Git Repository 

``` 
git clone https://github.com/rladiestaipei/R-basic.git
``` 

----

+ 執行 Git 的 3 個 States

----

+ Modified (修改檔案)
	+ 使用 git status 看那些檔案有變化
		``` 
		git status
		```
	+ 使用 git diff 看看改了什麼 

		```
		 git diff 
		```

----

+ Staging
	+ 改好了沒問題, 使用 git add 把檔案加入 staged

 ```
	 git add filename
	 git add . //加入全部被修改過的檔案
 ```

----

+  committed
	+ 使用 git commit 把 git 存入local repository
	```
	git commit -m "Add chapter 4"
	```
	+ 使用 git log 看看 git commit history
	```
	git log
	```

----

+ 上傳到遠端資料庫

    + 使用 git pull 將 github 上最新的版本與自己的本地端的合併
    ``` 
    git pull
    ```
    + 解決 Conflict
    + 使用 git push 把合併好的上傳到 github 
    ```
    git push
    ```
    + 可以使用 git log -r 檢查一下 github 上是不是有你改的部分
    ```
    git log -r
    ```

---

## 恭喜你，你已經可以使用 Git 跟 RLadies 協作了

---

## 情境 1 與 2 我都會了， 接下來 ?

---

## 在 local 與 Github 上建立 Repository 

---

## 取出某個版本: Git checkout

```
git checkout <hashnum>
git checkout e3ec69f
```

---

## 分支 : Git Branch
![](https://i.imgur.com/kJirkDi.png)

----

## Git branch command

```
## 列目前local 的 branches 跟所在 branch
git branch 

## 開一個新的 branch
git branch <branchname>

##  開一個新的 branch 並且checkout到那個 branch
git checkout -b <branchname>

```

----

## 分支管理 
----

![](https://i.imgur.com/oVkhAeS.png)

---

## 更多 : reset revert merge rebase  cherry-pick config ssh setup ...

---

## Q and A

---

## Thanks you!







