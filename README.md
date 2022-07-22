Hello git!

# 前言
哈囉，歡迎來到此地！
這裡是為 git 能力驗收而設置的場域，
任務會一一列舉在 `master-git-quiz` 的分支當中。
你必須將此分支當作主線，去作各種相對應的任務！

注意！不可使用圖形化 GUI 的 git 操作！


## 任務一 —— 測驗基礎遠端 github 能力
- 請以 `master-git-quiz` 分支為主線，開新的分支名為 `feature#1-empty-project`，並在 `README.md` 開頭打上 "Hello git!"
- 此外，commit 開頭請以 "[feature]" 開頭下評註，於第三行要有詳細的內容補充 commit 所做的事情，例如 "update README.md with a single line message".

全數完成後請直接推一個名為 "feature#1-empty-project" 的分支在本 repo 上。

## 任務二 —— 測驗基礎 Pull request 能力
- 分支 `feature#2-PR-practice` 上，有一個 `main.py` 檔案，並未符合 PEP8 標準規格，請你修改該檔案使其符合 PEP8，並繳交 PR 到 `master-git-quiz`，設定 reviewer 為 yuchen0515
- 注意
    - 格式請參考：https://github.com/yuchen0515/Data-Visualization-Project-Laptop-Sales/pull/22
    - 需有標籤 `dev`
    - 請隨意打上 comment，例如 "麻煩 @yuchen0515 協助 code review"

完成後，我會故意退回一次，請你修改，接著你必須打上 comment 說已經修復完畢，此時才算完成，然而我暫時先不會合併他，因為有下一個任務。

## 任務三 —— 練習 rebase interactive
- 我會隨機在 `feature#2-PR-practice` 加上四個 commit，按照時間順序分別為 A, B, C, D
- 請你先開分支儲存「備份」，分支名為 "feature#2-PR-practice-backup"
- 接著：
   - 合併 BC 為一個 commit
   - 修改 A 的 commit 為 "feature#1487 this commit complete"
   - 變更順位：D BC A
- 強行推上 `feature#2-PR-practice`，並觀察 Pull request 上的變化

## 任務四 —— 學會在 PR 鎖定分支 更新
- 當你完成任務三時，我會隨機在 `master-git-quiz` 新增 commit，這時 PR 頁面就會出現 "conflict" 而無法合併，你必須 "更新" 並與 master-git-quiz 一致，接著將你至今的 commit 抓回到這個分支上，意思就是先有 master-git-quiz 上的所有東西，至今多的 commit 則在其後

## 任務五 —— (進階) 修改特定變更為另一 commit
我會添加以下 commit：
- commit A：變更 README 特定兩個範圍之內容，例如 Line 20-40, 80-90, 變更 main.py 多 "hello git"
- commit B: main.py 多一 function

請你將 commit A 中針對 README 檔案的 Line 80-90 這個變更，改成 commit B 的變更，因此 commit B 會有兩項變更：
- README.md 80-90 變更
- main.py 多 function

此任務完成後，就會正式合併該 Pull request。

## 任務六 —— code review
我會以 新的 master-git-quiz 為基礎開新分支 "feature#3-code review"
接著會將 main.py 弄亂，發新 PR，設定 reviewer 為你

請一一檢視程式碼，給予 comment，將所有不符合 PEP8 標準的地方給予指正，並提示我修正之。當我確認你有全部抓到，我會再發一個全部改為 PEP8 的 code 上去。這時請你按照正常流程，給 approve comment，並以 "rebase" 方式合併，合併後點選按鈕 "delete" branch

## 任務七 —— 回到重前
請在不使用 reset, revert 的情況下，直接將 `master-git-quiz` 分支的東西，繳交一個 commit，需保留此 "README.md"(是有 Hello git 的版本)，其餘需完全和 `master` branch 內容完全一致。

額外條件：你繳交的這筆 commit 需有 "verify" 字樣！請自行上網查詢方法～

## 任務八 —— checkout 大師
請用 checkout 的方式，還原 README.md 為 "沒有 Hello git" 的版本，並繳交為新的一筆 verify commit。

## 結語
至此即認可有基礎的 git 能力，可參與團隊協作開發
並且擁有這樣的基本能力後，就能夠自己想出解法
也能自行在網路上學習
