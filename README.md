# Anxiety Tester

## 開發團隊
|Name|Education| Role
|:--|:--|:--|
|Yu-Chen Lin, mathlin| 師大資工系| 丁老師請我當指導者...會視情況變開發者|
|Hunter| 師大科技系| 開發者|
|Coding| 彰師工教系| 開發者|

- 角色定位之後再確認，看老師意思與說法
- 我想當糾察隊、架構檢視和研究新功能的傢伙，但 Python 開發經驗不算豐富，甚至連語法糖都還不會用，可能有點困難

## 開發細節
- Language: Python
- framework: [PyQt5](https://doc.qt.io/qtforpython/)
- UI/UX design tools: [figma](https://www.figma.com/)


## 協作方式
- 因應團隊規模小，而後續有持續維護與擴充之可能性，故以單一穩定分支 `master` 進行
- 原則上：都需在其他分支完成並測試好程式碼後，發 Pull Request 到 master
   - `WIP:` 尚未完成請在標題前方標記
   - Reviewer: 請安排至少一位以上自己以外的團隊人員。
   - code review: 請給 Reviewer 看過，有問題須在相應程式碼 comment 退回給當事人修改，reviewer 無需擔當問題解決者，反覆來回直到無問題才可合進 master。
   - reviewer 請在合成前，確認 master 與當前分支的 commit 狀況，以 rebase 為主，不要因為 merge branch 製造無謂的 commit。
- 除了 master 以外的分支
   - 確認當前只有你在做事時，允許使用 `-f` 強迫推行。
   - 可以不用很乾淨，但發 MR 時，請務必用 `git rebase -i` 整理好 commit 再發 MR。
- 分支種類
   - `feature` - 開發功能使用
   - `bugfix` - 修復某一問題使用
   - `hotfix` - 緊急修復問題時使用
   - `format` - 修改程式碼格式時使用，請勿在你開發某功能時，「順便」幫其他程式碼 formatting
- Pull Request (PR)
   - title
      - 若為半成品開頭標記 `WIP:`
      - 按開發種類標記，如：`Feature #1 - added camara frame`，編號看所屬種類 PR 送到幾號依此遞增
   - content 請包含三大內容，包含但不限於此三大內容，可自行補充
      - 目的 & 功能: 請說明這個 PR 做的事情，加了什麼功能？或想達到什麼目的？
      - 更動：請一一列出所有修改、新增和刪除的檔案，包含檔案的**絕對**路徑
      - 驗證：如果是介面效果，請截圖貼上你的效果。總之對於你這個 PR 做的事情盡量能有驗證畫面或驗證 API。有些功能自然是沒有就不需要，例如修改格式之類的。
- 資料夾
   - 規定 source code 一律放 `/src` 資料夾下
   - 沒有特別的其他規定，希望是參考其他 pyqt5 github 上開發的大專案框架下去操作


## 格式要求
- 請遵循 Python [PEP8](https://peps.python.org/pep-0008/) style
- 盡量包裝成 class，你的目標是沒參與你 feature 開發的人，可以不用知道你的 class 做哪些事，但他卻有辦法使用、操作，可以想像你是開發者，使用你的 class 的都是用戶，不能預設他什麼都知道。

